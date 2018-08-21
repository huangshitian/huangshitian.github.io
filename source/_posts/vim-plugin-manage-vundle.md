---
title: vim插件管理 Vundle
tags: vim
date: 2018-08-19 16:04:05
---


# Install Vundle and Vundle commands

## Install
	First you must have vim and git software.

	* git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
	* add config to top of ~/.vimrc

	`
		see the website: https://github.com/VundleVim/Vundle.vim
	`

## Commands

:PluginInstall 	安装命令
:PluginInstall!	重新安装所有插件
:bdelete		deleteBuffer
:PluginSearch	查找插件
:PluginSearch!	强制刷新本地缓存列表，进行查找
:PluginList		查看所有已安装的插件
:PluginUpdate	更新插件
:PluginClean	清除无效的插件

## cmd-line
vim +PluginInstall +gall

## config Plugin And add Plugin

add plugin config between "call vundle#begin" and "call vundle#end()"

Plugin in github repository.

example: `Plugin	'tpope/vim-fugitive'`

not in github need full url

example: `Plugin 'git://git.wincent.com/command-t.git'`
