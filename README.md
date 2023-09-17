# pgsql.vim
Vim syntax file for PostgreSQL
==============================

* Language:	pgsql
* Maintainer:	Devrim Gündüz <devrim@PostgreSQL.org>
* Last Change:	$Sun 17 Sep 11:48:07 BST 2023$
* Filenames:	*.pgsql *.plpgsql
* URL:		ttps://github.com/devrimgunduz/pgsql.vim

Installation
---

Copy `pgsql.vim`  into your `~/.vim/syntax/` directory, creating it if necessary.

Usage
---

Files with the suffix `.pgsql` will use the pgsql highlighting automatically.

To enable `pgsql` syntax for any open buffer, use:

    :set syntax=pgsql

Enabling for all .sql files
---

You can make `pgsql.vim` the default for SQL syntax by adding this line to your
`.vimrc`:

    let g:sql_type_default = 'pgsql'

This tells the `sql.vim` module to use the `pgsql` dialect.

Alternately, you can use an autocmd in your `~/.vim/filetype.vim` to enable it
for all `.sql` files or some finer pattern:

    autocmd BufNewFile,BufRead *.sql setf pgsql

You do not need both. If in doubt, use the first method.
