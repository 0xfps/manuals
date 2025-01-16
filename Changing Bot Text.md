# Changing Bot Text

1. Get in to your console as described [here](./Starting And Stopping Bot.md).
2. Run:

```bash
pm2 list
```

3. If the list is empty, proceed with step 5.
4. If the list is not empty, run:

```bash
pm2 stop all
```

```bash
pm2 delete all
```

5. Run:

```bash
vi src/messenger/parse-message.ts
```

6. Press the `i` button on your keyboard.
7. Change the text in the section with "PepeBuldak Sales Live".
8. Press the `Esc` button on your keyboard.
9. Press `:wq!` and hit `Enter`.
10. Run

```bash
npm run clean
```

11. Run

```bash
pm2 start build/index.js
```
