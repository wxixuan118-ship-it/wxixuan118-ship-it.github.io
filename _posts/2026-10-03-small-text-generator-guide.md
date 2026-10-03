---
layout: post
title: "Small Text Generator Guide: Small Caps, Superscript, Subscript and Discord Subtext"
description: "Small text generator guide: how small caps, superscript and subscript work, missing letters, platform support and Discord -# subtext."
date: 2026-10-03 15:50:00 +0800
tags: [unicode, discord, typography]
---

ᴛɪɴʏ ʟᴇᴛᴛᴇʀꜱ, ˢᵘᵖᵉʳˢᶜʳⁱᵖᵗ and ₛᵤᵦₛ꜀ᵣᵢₚₜ all look like "small text", but they come from different parts of Unicode and behave differently once you paste them. A small text generator hides those differences behind a single text box, which is convenient until a letter refuses to shrink or a username field rejects your text.

This guide explains the three main kinds of tiny text, why some letters are missing in each style, where small text works, and when Discord's built-in `-#` subtext is the better option.

## Small text is Unicode characters, not a smaller font

Most apps don't let you change font size in a bio or display name. Small text gets around that by replacing each normal letter with a different character that is drawn smaller. Because the change lives in the characters themselves, it survives copy and paste into any field that accepts plain text.

That also means a small text generator is really a lookup table: `a` becomes `ᴀ`, `ᵃ` or `ₐ` depending on the style you pick. Which table you use decides how complete and readable the result is.

## The three kinds of small text

### Small caps (ꜱᴍᴀʟʟ ᴄᴀᴘꜱ)

Small caps are capital-letter shapes at lowercase height. They sit on the normal baseline, so they read naturally in a sentence and are the easiest of the three styles to read.

Most of these characters come from Unicode's phonetic alphabets, where linguists use small capitals as sound symbols. That history explains the gaps:

- There is **no small capital X** in Unicode, so generators fall back to a plain `x`.
- A small capital Q (`ꞯ`) was added only in Unicode 11, and some fonts still don't include it.

### Superscript (ᵗⁱⁿʸ ᵗᵉˣᵗ)

Superscript letters are raised above the baseline. This is the classic "tiny text" look used in bios and comments, and it is the smallest of the three styles on most screens.

Coverage is nearly complete. Most letters come from the "modifier letter" set, while `ⁱ` and `ⁿ` sit in the Superscripts and Subscripts block. The awkward one is **q**: a superscript q (`𐞥`) exists only in recent Unicode versions and is rarely supported by fonts, so many generators substitute a look-alike or leave q unchanged.

### Subscript (ₛᵤᵦₛ꜀ᵣᵢₚₜ)

Subscript letters drop below the baseline, as in chemical formulas like H₂O. Unicode only encodes subscript versions of some Latin letters:

```text
Available:  a e h i j k l m n o p r s t u v x
Missing:    b c d f g q w y z
```

Generators fill some gaps with look-alikes. In "ₛᵤᵦₛ꜀ᵣᵢₚₜ", for example, the `ᵦ` is a Greek subscript beta and the `꜀` is a Chinese tone mark that happens to look like a small c. Others leave the missing letters full-size. Subscript works well for numbers (₀₁₂₃) and short scientific notation, but whole words in subscript usually come out uneven.

## Where small text works, and where it doesn't

Small Unicode text generally renders on modern phones, browsers and desktop systems. Problems usually come from the field, not the font:

- **Bios, captions and display names** on Instagram, TikTok, X and Discord typically accept these characters.
- **@usernames and handles** on many platforms only allow plain letters, numbers and a few symbols, so styled text is rejected or stripped.
- **Very old devices** may show a few rare characters, such as the newer small capital Q, as empty boxes.

Always paste the result into the actual field and preview it before saving. The [small text generator on MiniTextGenerator](https://minitextgenerator.com/) shows small caps, superscript and subscript side by side, which makes it quick to see which style keeps every letter of your text.

## Discord's -# subtext vs Unicode tiny text

Discord has its own way to make text smaller. Start a message line with `-#` followed by a space, and Discord renders that line as small, muted subtext:

```text
-# this line shows up as small grey text
```

Subtext and Unicode tiny text solve different problems:

| | Discord `-#` subtext | Unicode small text |
|---|---|---|
| Works in | Discord messages only | Anywhere plain text is accepted |
| Letters | Normal letters, so fully readable and searchable | Look-alike characters, some letters missing |
| Display names and status | No, markdown doesn't apply there | Yes, in fields that accept Unicode |
| Copy to other apps | Becomes plain text with `-#` | Keeps the small look |

Use `-#` for footnotes, disclaimers and quiet asides inside Discord chat. Use Unicode small text for nicknames, server names, status messages and anything outside Discord. MiniTextGenerator has a separate guide to [small text for Discord](https://minitextgenerator.com/small-text-discord/) that covers which Discord fields accept which style.

## Readability, search and accessibility

Tiny text is decoration, and it carries the same trade-offs as other Unicode styling:

- **Search.** Platforms may not match `ꜱᴍᴀʟʟ` when someone searches for "small". Unicode NFKC normalization folds superscript and subscript letters back to plain letters, but it leaves small caps unchanged, so even systems that normalize text may treat small caps as different words.
- **Screen readers** may read these characters by their symbol names or skip them, which turns a short bio into noise.
- **Legibility.** Superscript at small font sizes is hard to read on phones, especially for longer phrases.

Keep small text to a word or a short phrase, and never use it for information people need to find or understand.

## FAQ

### Why does my small text generator skip some letters?

Unicode has no small version of every letter. Subscript is missing b, c, d, f, g, q, w, y and z, small caps has no x, and superscript q is poorly supported. Generators either substitute look-alikes or leave those letters full-size.

### Which small text style is the smallest?

Superscript usually looks smallest because it is both reduced and raised. Small caps are larger but easier to read. Which is smallest also depends on the platform's font.

### Can I use small text in my Discord name?

Usually yes for your display name, server nickname and status, which accept Unicode. Your @username only allows plain characters. The `-#` subtext markdown only works inside messages.

## Conclusion

A small text generator gives you three different alphabets: small caps for readability, superscript for the tiniest look, and subscript mainly for numbers and formulas. Each has gaps that come straight from Unicode, so preview your text in the field where it will live. On Discord, reach for `-#` subtext in messages and Unicode tiny text everywhere else. To compare all three styles with your own words, try the free [small text generator](https://minitextgenerator.com/).
