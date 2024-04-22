# inventory-management-system

個人向け物品管理システム

# 制作の背景

1. ビジネス化(~~転売~~)を視野にヲタクグッズを集めすぎており、推定 2000 点以上ある
2. 暫定的に Google Spread Sheet 上で管理しているが、不便になってきたし発展に限界があるので、データを RDB に移行して管理画面経由で操作したい。

# Todo

1. RDB 設計
2. Google Spread Sheet から RDB への移行
3. 開発環境整備(Docker)

# 技術要件

某所の技術スタックの素振りを兼ねているためそちらを採用する。

- Laravel
- Blade
- vue.js(ver2)

ただし DB は下記の SaaS に合わせざるをえない。

# 本番環境選定

なんといってもホビーなので無料で運用したい。
DB に関しては SaaS 使うかも

- [supabase(postgreSQL)](https://supabase.com/)
- [neon(postgreSQL)](https://neon.tech/)
- [turso(SQLite)](https://turso.tech/)
- [CockroachDB](https://www.cockroachlabs.com/lp/serverless/)
- [AWS RDS(MySQL)](https://aws.amazon.com/jp/rds/)
