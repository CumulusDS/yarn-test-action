[![Create Release][release-badge]][release-url]
[![Import Labels][import-labels-badge]][import-labels-url]
[![Sync Labels][sync-labels-badge]][sync-labels-url]
[![PR AutoLabeler][autolabeler-badge]][autolabeler-url]
[![Assigner][assigner-badge]][assigner-url]

Simplify Workflow Jobs by combining steps into a single [composite action][Composite Action].

Replaces the following:

```yaml
      - name: Check licenses
        run: yarn build:license-checker
      - name: Start Flow Server
        run: yarn flow start
      - name: Test
        run: yarn test
````

with

```yaml
      - name: Yarn Test
        uses: CumulusDS/yarn-test-action@master
```

[Composite Action]: https://docs.github.com/en/actions/creating-actions/creating-a-composite-action
[release-badge]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/release.yml/badge.svg
[release-url]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/release.yml
[import-labels-badge]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/labels_import.yml/badge.svg
[import-labels-url]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/labels_import.yml
[sync-labels-badge]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/labels_sync.yml/badge.svg
[sync-labels-url]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/labels_sync.yml
[autolabeler-badge]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/autolabeler.yml/badge.svg
[autolabeler-url]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/autolabeler.yml
[assigner-badge]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/assign.yml/badge.svg
[assigner-url]: https://github.com/CumulusDS/yarn-test-action/actions/workflows/assign.yml
