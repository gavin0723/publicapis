#encoding=utf8
#
# 	Copyright 2016 北京大数医达科技有限公司
#

.PHONY: python go

CurrentDir := $(RootWorkDir)/api/iyoudoctor/partner/mercury/drug

python:
	@# Ensure the directory
	mkdir -p $(PythonGenPath)/iyoudoctor/partner/mercury/drug
	@# Run sub modules
	@$(MAKE) -C $(CurrentDir)/v1 python
	@#Create the __init__.py
	touch $(PythonGenPath)/iyoudoctor/partner/mercury/drug/__init__.py

go:
	@$(MAKE) -C $(CurrentDir)/v1 go
