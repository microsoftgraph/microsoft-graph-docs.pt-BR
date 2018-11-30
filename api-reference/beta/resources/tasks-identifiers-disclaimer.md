---
title: Identificadores de tarefas
description: 'Identificadores de objetos em tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores são 28 caracteres de comprimento e diferenciam maiusculas de minúsculas. Quando passados como no, o serviço fará uma validação de formato simples do identificador, se o formato validação falhar, os chamadores receberá uma resposta de erro de solicitação incorreta (400) indicando esse problema. Receber esse erro indica um bug do aplicativo de chamada, tais como:'
ms.openlocfilehash: d57ca282de87c2bce42b37d0be6d08dbe128c522
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040795"
---
# <a name="identifiers-in-tasks"></a>Identificadores de tarefas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Identificadores de objetos em tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores são 28 caracteres de comprimento e diferenciam maiusculas de minúsculas. Quando passados como no, o serviço fará uma validação de formato simples do identificador, se o formato validação falhar, os chamadores receberá uma resposta de erro de solicitação incorreta (400) indicando esse problema. Receber esse erro indica um bug do aplicativo de chamada, tais como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres que não diferencia maiúsculas de minúsculas. Os identificadores em Tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncou o identificador. Os identificadores em Tarefas têm 28 caracteres.
- O aplicativo de chamada tentou gerar um valor do identificador para um objeto em Tarefas. Não são aceitos identificadores gerados por clientes. Todos os identificadores são gerados pelo serviço durante a criação de objetos.

A validação **não é um recurso de segurança**. Ela serve para informar os aplicativos sobre problemas comuns relacionados aos identificadores durante o desenvolvimento do aplicativo que, caso contrário, seriam difíceis de identificar.