# UpdateVersion

_A github action to manage version numbers for pip installable packages for private repos_

## Use

To call in your workflow, add the following step to any job

```github
        steps:
          - name: Update Version
            uses: byusawsfhtl/UpdateVersion@v1.0.2
            with:
              token: ${{ secrets.YOUR_BOT_TOKEN_NAME_HERE }}
```

## Requirements

This action requires one to keep their version number in a `_version.py` file in the root directory of the project.

As shown above, a token for a bot to create commits with is also required. The bot must be able to automatically push commits into branches.