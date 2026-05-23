POETRY := $(shell command -v poetry 2>/dev/null || echo /Users/redwolf18/.local/bin/poetry)

install:
	$(POETRY) install

pre-commit-install:
	$(POETRY) run pre-commit install

lint:
	$(POETRY) run pre-commit run --all-files

repro:
	$(POETRY) run dvc repro

clean:
	rm -rf data/processed models metrics reports
