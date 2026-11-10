<h1 align="center">
  <img src="https://avatars1.githubusercontent.com/u/29598503?v=3&s=256" alt="INADYN">
  <br />
  INADYN
  <br />
</h1>

<p align="center"><b>This is the snap for INADYN</b>, <em>"Internet Automated Dynamic DNS Client"</em>. It works on Ubuntu, Fedora, Debian, and other major Linux distributions.</p>

<p align="center">
<a href="https://snapcraft.io/inadyn">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/static/images/badges/en/snap-store-black.svg" />
</a>
</p>

## Install

    sudo snap install inadyn

([Don't have snapd installed?](https://snapcraft.io/docs/core/install))

## Configuration

The snap stores its configuration in `$SNAP_DATA/inadyn.conf`. Find the current path with:

    inadyn.configpath

Edit that file using the [upstream configuration documentation](https://github.com/troglobit/inadyn#configuration), then restart the service:

    sudo snap restart inadyn.daemon

## How to contribute

### Reporting issues

Please [open an issue](https://github.com/snapcrafters/inadyn/issues/new) if you find a bug, have a feature request, or if the snap is out of date.

### Updating the snap

Snap versions are [automatically kept in sync](https://github.com/snapcrafters/inadyn/actions/workflows/sync-version-with-upstream.yml) with upstream releases. To update it manually, [open a pull request](https://github.com/snapcrafters/inadyn/compare) against `candidate`.

When the pull request is merged, the release workflow builds and publishes to `latest/candidate` and opens a call for testing. After testing, a maintainer can promote the snap to stable.

### Testing

Subscribe to the [candidate channel](https://snapcraft.io/inadyn) and [leave a comment](https://github.com/snapcrafters/inadyn/issues) with your results.

    sudo snap install inadyn --channel=candidate

### Maintainers

- [Snapcrafters](https://github.com/snapcrafters)

## License

The scripts and documentation in this project are released under the [MIT License](LICENSE).
