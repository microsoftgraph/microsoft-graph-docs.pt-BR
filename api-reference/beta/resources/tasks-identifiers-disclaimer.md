---
title: Identificadores de tarefas
description: 'Identificadores de objetos em tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores são 28 caracteres de comprimento e diferenciam maiusculas de minúsculas. Quando passados como no, o serviço fará uma validação de formato simples do identificador, se o formato validação falhar, os chamadores receberá uma resposta de erro de solicitação incorreta (400) indicando esse problema. Receber esse erro indica um bug do aplicativo de chamada, tais como:'
localization_priority: Normal
ms.openlocfilehash: 98a999fa2473a8f77b316d6acf668aec9c3ac832
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527609"
---
# <a name="identifiers-in-tasks"></a>Identificadores de tarefas

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Identificadores de objetos em tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores são 28 caracteres de comprimento e diferenciam maiusculas de minúsculas. Quando passados como no, o serviço fará uma validação de formato simples do identificador, se o formato validação falhar, os chamadores receberá uma resposta de erro de solicitação incorreta (400) indicando esse problema. Receber esse erro indica um bug do aplicativo de chamada, tais como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres que não diferencia maiúsculas de minúsculas. Os identificadores em Tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncou o identificador. Os identificadores em Tarefas têm 28 caracteres.
- O aplicativo de chamada tentou gerar um valor do identificador para um objeto em Tarefas. Não são aceitos identificadores gerados por clientes. Todos os identificadores são gerados pelo serviço durante a criação de objetos.

A validação **não é um recurso de segurança**. Ela serve para informar os aplicativos sobre problemas comuns relacionados aos identificadores durante o desenvolvimento do aplicativo que, caso contrário, seriam difíceis de identificar.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/tasks-identifiers-disclaimer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
