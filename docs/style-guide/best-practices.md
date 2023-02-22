# Guidelines and best practices

Review these guidelines before you begin authoring content.

## Writing best practices

- Write content from a 2nd-person perspective. You're explaining to the user what they need to do. Address them as *you*, not *the user* or anything else.
- Shorter is better. Less is more. Write concisely and briefly. If you're unsure, pick the *shorter* option.
- Avoid "the following", "above", and "below". Just use a colon to introduce what's next.
- Use common contractions (isn't, aren't, don't, and so on) to increase readability, or *don't* use contractions to increase formality. Most importantly, be consistent in enforcing whichever method you choose.
- Review [everyday language (EDL)](voice-tone.md#everyday-language-edl) and [language choices](language-choices.md).
- Avoid FAQs. Put that information where users need it, such as in the tutorial steps.

## Content organization

- Tutorials use *numbered steps*, because they explain how to complete a task. Use numbered steps for sequential items and bulleted lists for non-sequential items.
- Use hyphens (`-`), not asterisks (`*`), for bullets. Ensure all list items end with a period if even one item contains more than three words.
- File names must use *only* lowercase letters and hyphens. *No uppercase letters or underscores should be used*. Use names that resemble the H1 for the topic (for example, `create-new-user.md` and `create-user-step-1.jpg`).
- *Don't* use HTML, except for the following exceptions:
    - You can use the `<br>` tag to force line breaks.
    - You can use the `<ul>`/`<ol>` and `<li>` tags to create bulleted or numbered lists within Markdown tables.
    - You can use HTML entities (such as `&rarr;`, `&larr;`, `&copy;`, `&#154;`, and so on).
    - You can use the `<u>` tag to underline text.
    - *No other HTML should be used*.

## Markdown usage

Follow these best practices when writing with Markdown.

### UI elements and emphasis

- Only use **bold** to introduce bulleted items and interface/UI elements. Use *italics* for emphasis.
- Don't click on tabs. *Select* them. For drop-down menus, use *choose*. For everything else, use *click* and not *click on*:

    | Use | Don't use |
    |---|---|
    | Click **Generate report**. | Click on **Generate report**. |
    | Click **Migrate**. | Click the **migrate** button. |
    | Select the **Reports** tab. | Click on the **Reports** tab. |

- Use single asterisks around a word (`*`) for italics. Don't use underscores (`_`).
- Use single backticks for code phrases and terms. Use backticks for phrases that include underscores, as these will otherwise render as italics. (Example: `THIS_CODE_PHRASE`).

### Headings

- Every topic should start with an H1 (`#`) and then change sequentially; don't jump from an H2 (`##`) to an H4 (`####`).
- Only one H1 (`#`) per page. Follow your H1 with an introductory paragraph that explains the topic.
- Don't use bold for headings. Use pound signs (`#`).
- Use up to heading level four when necessary. If you have to go deeper, consider restructuring your docs.
- Avoid punctuation and links in headings.
- Headings in the topic and the ToC should be in sentence case (like this sentence). ToC headings should match or resemble the H1 heading for the linked topic.
- Tutorial headings should start with a verb. Concept and reference topics can be named to match the concept you're describing or the content you're providing for reference.

| Use | Don't use |
|---|---|
| Create a user | How to create a user |
| Migrate to AWS | AWS migration |
| Workflow architecture | Understanding the workflow architecture |
| Environments | List of environments |

### Code blocks

- Use fenced code blocks. This means using three backticks to open the code block and three more to close it. For example:

    ```
        ```
        public function __construct() {
            $this->user = new User();
        }
        ```
    ```

- Make sure you include the language used within the code block after the first backticks. For a list of supported languages, see [Prism supported languages](https://prismjs.com/#supported-languages).
- Inline code snippets only require a single backtick, for example:

    ```
        `line-of-code`
    ```

### Links

- For links with placeholders that only serve as examples, wrap them in backticks. Otherwise, they may not pass validation tests.
- When linking to a different topic, use its actual name instead of "click here".
- Don't leave bare URLs in your Markdown. Make them hyperlinks or wrap them with angle brackets.

| Use | Don't use |
|---|---|
| `[Google](https://google.com)` | `[Click here](https://google.com)` |
| `<https://google.com>` | `https://google.com` |

## Document architecture

- Ensure every page has an introductory sentence for *each* heading on the page. You can't have the title of the document, then an H2, for example.
- Ensure every page has a *More info* section (or a *Next step* section for getting started topics) at the end that containing at least two relevant links.

## Practical guidelines

Follow these best writing practices to ensure your content is clear and concise:

- Use headings correctly — they should follow a clear hierarchical structure. Don't repeat heading titles.
- Use lists for readability — use bulleted lists for a list with unordered entries and a numbered list for sequential items. Don't make your page one giant list, if possible, and avoid nesting deeper than two levels, with three being the max.
- Use tables to organize information that's referenced by the reader.
- Write in the second person — refer to the user as *you*.
- Avoid "should" or "will happen" statements. Write in the active voice and as if processes work perfectly.
- Use diagrams appropriately.
- Keep it short and simple.
- Define your terms and acronyms the first time they appear in your topic.

## More info

- [Grammar and mechanics](grammar-mechanics.md)
- [Language and choices](language-choices.md)
- [Voice and tone](voice-tone.md)
- [Interface items and standards](interface-items-standards.md)
