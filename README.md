# Asynchronous-Programming-with-Asyncio
Demonstrates asynchronous programming using the asyncio library.
import asyncio

async def greet(name):
    print(f"Hello, {name}!")
    await asyncio.sleep(2)
    print(f"Goodbye, {name}!")

async def main():
    await asyncio.gather(greet('Alice'), greet('Bob'))

asyncio.run(main())
