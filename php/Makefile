.PHONY: install
install:
	composer update

.PHONY: phpstan
phpstan:
	vendor/bin/phpstan analyse -c phpstan.neon

.PHONY: tests
tests:
	vendor/bin/tester -s -p php --colors 1 -C tests/Cases

.PHONY: coverage
coverage:
	vendor/bin/tester -s -p phpdbg --colors 1 -C --coverage coverage.html --coverage-src src tests/Cases
