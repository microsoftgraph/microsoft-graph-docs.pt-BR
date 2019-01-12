---
title: Identificadores no Planner
description: 'Identificadores de objetos no planejador são valores de cadeia de caracteres gerados pelo serviço. Os valores são 28 caracteres de comprimento e diferenciam maiusculas de minúsculas. Quando passados como no, o serviço fará uma validação de formato simples do identificador, se o formato validação falhar, os chamadores receberá uma resposta de erro de solicitação incorreta (400) indicando esse problema. Receber esse erro indica um bug do aplicativo de chamada, tais como:'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75c284d576ed6f03691828309fab7ed899c1c066
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951851"
---
# <a name="identifiers-in-planner"></a>Identificadores no Planner

Identificadores de objetos no planejador são valores de cadeia de caracteres gerados pelo serviço. Os valores são 28 caracteres de comprimento e diferenciam maiusculas de minúsculas. Quando passados como no, o serviço fará uma validação de formato simples do identificador, se o formato validação falhar, os chamadores receberá uma resposta de erro de solicitação incorreta (400) indicando esse problema. Receber esse erro indica um bug do aplicativo de chamada, tais como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres que não diferencia maiúsculas de minúsculas. Os identificadores em Tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncou o identificador. Os identificadores em Tarefas têm 28 caracteres.
- O aplicativo de chamada tentou gerar um valor do identificador para um objeto em Tarefas. Não são aceitos identificadores gerados por clientes. Todos os identificadores são gerados pelo serviço durante a criação de objetos.

A validação **não é um recurso de segurança**. Ela serve para informar os aplicativos sobre problemas comuns relacionados aos identificadores durante o desenvolvimento do aplicativo que, caso contrário, seriam difíceis de identificar.
