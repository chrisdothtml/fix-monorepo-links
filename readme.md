# fix-monorepo-links

## Purpose

- Replaces package URLs with their new location in the monorepo
- Updates `package.json` -> `repository` & `homepage`
- Removes buildkite status badges

## Use

### 1. Install deps

```sh
yarn
```

### 2. Navigate to the directory with your packages

```sh
cd ../my-monorepo/packages
```

### 3. Run

```
Usage: ../../fix-monorepo-links/fix [args]

Required args
  --monorepo: `owner/name` format
  --org: github org name repos came from

Optional args
  --subDir: subdirectory of the packages (used for package homepage url)

Examples
  fix --org=fusionjs --monorepo=fusionjs/fusion --subDir=packages
```
