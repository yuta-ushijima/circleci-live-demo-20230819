# circleci-live-demo-20230819
- CircleCIで下記のworkflowを実行するサンプルリポジトリです

## Workflow
1. リポジトリにコードをpush
2. CircleCIがリポジトリにpushされたことをイベントトリガーとしてworkflowを実行
3. 最初のworkflowとしてCloudformationを実行
4. 2番目のworkflowとして、Cloudformationによって作成されたAWS環境に対してansibleを実行
5. 3番目のworkflowとしてServerspecによる自動テストを実行する

## 実行環境
### aws cli
```bash
2.11.26
```

### ansible
```bash
2.10.7
```

### ruby
```bash
3.2.2
```