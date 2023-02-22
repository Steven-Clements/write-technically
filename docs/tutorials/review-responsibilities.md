# Merge request review responsibilities

Be sure that at least one person reviews your work before deploying it to production. This page lists the responsibilities of both the author and the reviewer.

## Writer responsibilities

Before submitting a merge request (MR) for review, the writer should:

1. Create a *draft* MR for the review, and notify other team members what should be reviewed.
2. Run MkDocs locally by entering the following command into a Command Prompt:

    ```
    mkdocs serve
    ```

    > **NOTE**: You must navigate to the directory that contains the `docs` directory and `mkdocs.yml` file for your documentation by using the change directory (`cd`) command before using this code snippet.

3. Review the Mkdocs build at `http://127.0.0.1:8000` (or `http://localhost:8000`), and confirm that the ToC is rendering correctly, all images display correctly, and all links resolve as expected.
4. Confirm that file and image names are human-readable.
5. Confirm that *More info* links exist on each topic (or *Next step* for getting started topics).
6. Ensure that all sentences longer than three words end with a period, including sentences within bulleted and numbered lists.
7. Fix any issues (spacing, list formatting, and so on) highlighted by the linter.
8. Mark the MR as ready to merge after all of your changes are in.

## Reviewer responsibilities

After the MR is submitted for review, the reviewer should:

1. Tell the team that wrote the documentation that you're about to start a review on the project, and ask their team to hold all updates.
2. Pull the branch to your local environment.
3. Run `mkdocs serve` locally and confirm that no build issues occur.
4. Review the Mkdocs build at `http://127.0.0.1:8000` (or `http://localhost:8000`), and confirm that the ToC is rendering correctly, all images are displaying, and all links resolve as expected.
5. Confirm that file and image names are human-readable.
6. Confirm that *More info* links exist on each topic (or *Next step* for getting started topics).
7. Check for periods at the end of each list item.

## More info

- [Follow the Git workflow](git-workflow.md)
- [Style Guide](../style-guide/best-practices.md)
