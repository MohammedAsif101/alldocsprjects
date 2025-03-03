import pygame
import random
import time

# Initialize pygame
pygame.init()

# Define the game window
width = 600
height = 400
screen = pygame.display.set_mode((width, height))
pygame.display.set_caption('Snake Arcade Game')

# Define colors
white = (255, 255, 255)
yellow = (255, 255, 102)
black = (0, 0, 0)
red = (213, 50, 80)
green = (0, 255, 0)
blue = (50, 153, 213)

# Define fonts
font_style = pygame.font.SysFont("bahnschrift", 25)
score_font = pygame.font.SysFont("comicsansms", 35)

# Set the clock
clock = pygame.time.Clock()

# Define the snake block size and speed
block_size = 10
snake_speed = 15

# Function to display the score
def Your_score(score):
    value = score_font.render("Your Score: " + str(score), True, black)
    screen.blit(value, [0, 0])

# Function to draw the snake
def our_snake(block_size, snake_body):
    for x in snake_body:
        pygame.draw.rect(screen, green, [x[0], x[1], block_size, block_size])

# Function to draw the food
def food_spawn():
    return [random.randrange(1, (width // block_size)) * block_size, random.randrange(1, (height // block_size)) * block_size]

# Function to display messages on the screen
def message(msg, color):
    mesg = font_style.render(msg, True, color)
    screen.blit(mesg, [width / 6, height / 3])

# Main game loop
def gameLoop():
    game_over = False
    game_close = False

    # Snake starting position
    x1 = width / 2
    y1 = height / 2
    x1_change = 0
    y1_change = 0

    # Snake body initialization
    snake_body = []
    length_of_snake = 1

    # Spawn food
    food = food_spawn()

    score = 0

    while not game_over:

        while game_close:
            screen.fill(blue)
            message("You Lost! Press Q-Quit or C-Play Again", red)
            Your_score(length_of_snake - 1)
            pygame.display.update()

            for event in pygame.event.get():
                if event.type == pygame.KEYDOWN:
                    if event.key == pygame.K_q:
                        game_over = True
                        game_close = False
                    if event.key == pygame.K_c:
                        gameLoop()

        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                game_over = True
            if event.type == pygame.KEYDOWN:
                if event.key == pygame.K_LEFT:
                    x1_change = -block_size
                    y1_change = 0
                elif event.key == pygame.K_RIGHT:
                    x1_change = block_size
                    y1_change = 0
                elif event.key == pygame.K_UP:
                    y1_change = -block_size
                    x1_change = 0
                elif event.key == pygame.K_DOWN:
                    y1_change = block_size
                    x1_change = 0

        # Check if snake hits the boundaries
        if x1 >= width or x1 < 0 or y1 >= height or y1 < 0:
            game_close = True

        x1 += x1_change
        y1 += y1_change
        screen.fill(blue)

        # Draw the food
        pygame.draw.rect(screen, yellow, [food[0], food[1], block_size, block_size])

        # Update the snake's body
        snake_head = []
        snake_head.append(x1)
        snake_head.append(y1)
        snake_body.append(snake_head)
        if len(snake_body) > length_of_snake:
            del snake_body[0]

        # Check if the snake collides with itself
        for x in snake_body[:-1]:
            if x == snake_head:
                game_close = True

        our_snake(block_size, snake_body)
        Your_score(length_of_snake - 1)

        pygame.display.update()

        # Check if the snake eats the food
        if x1 == food[0] and y1 == food[1]:
            food = food_spawn()
            length_of_snake += 1
            score += 1

        clock.tick(snake_speed)

    pygame.quit()
    quit()

# Function to display the start screen
def start_game():
    screen.fill(blue)
    message("Press S to Start the Game", green)
    pygame.display.update()

    waiting_for_start = True
    while waiting_for_start:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                pygame.quit()
                quit()
            if event.type == pygame.KEYDOWN:
                if event.key == pygame.K_s:
                    gameLoop()

start_game()
