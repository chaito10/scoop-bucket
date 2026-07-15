# 📦 scoop-bucket

A personal Scoop bucket containing manifests for Windows applications maintained by **Charudatta Korde**.

## Installation

Add this bucket:

```powershell
scoop bucket add chaito10 https://github.com/chaito10/scoop-bucket
```

Install an application:

```powershell
scoop install chaito10/<app>
```

Update the bucket:

```powershell
scoop update
scoop update *
```

## Available Packages

List all manifests in this bucket:

```powershell
scoop search chaito10/
```

Or browse the `bucket/` directory in this repository.

## Repository Structure

```text
bucket/
├── app1.json
├── app2.json
└── ...
```

Each manifest follows the official Scoop manifest format and contains metadata, download URLs, hashes, and installation instructions.

## Contributing

Issues and pull requests are welcome.

When contributing a new manifest:

* Use valid Scoop manifest syntax.
* Include SHA256 hashes.
* Prefer official download sources.
* Test the manifest with:

```powershell
scoop install <manifest>
```

## Development

Validate manifests before submitting changes.

Useful commands:

```powershell
scoop bucket list
scoop search <package>
scoop info <package>
scoop install <package>
scoop uninstall <package>
```

These commands are part of the standard Scoop workflow.

## License

Unless otherwise specified, the manifests in this repository are released under the MIT License.

Package licenses remain the property of their respective authors.
