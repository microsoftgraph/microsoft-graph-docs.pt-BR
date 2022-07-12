---
title: Identificadores em Tarefas
description: 'Os identificadores de objetos em Tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores têm 28 caracteres e diferenciam maiúsculas de minúsculas. Quando passado como dentro, o serviço fará uma validação de formato simples do identificador. Se a validação do formato falhar, os chamadores receberão uma resposta de erro de Solicitação Incorreta (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:'
ms.localizationpriority: medium
doc_type: conceptualPageType
ms.prod: tasks-and-plans
author: TarkanSevilmis
ms.openlocfilehash: 4bac8d2fca466da934ac55b16c09c6c1d0977d32
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732692"
---
# <a name="identifiers-in-tasks"></a>Identificadores em Tarefas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os identificadores de objetos em Tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores têm 28 caracteres e diferenciam maiúsculas de minúsculas. Quando passado como dentro, o serviço fará uma validação de formato simples do identificador. Se a validação do formato falhar, os chamadores receberão uma resposta de erro de Solicitação Incorreta (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres que não diferencia maiúsculas de minúsculas. Os identificadores em Tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncadou o identificador. Os identificadores em Tarefas têm 28 caracteres.
- O aplicativo de chamada tentou gerar um valor de identificador para um objeto em Tarefas. Identificadores gerados pelo cliente não são aceitos. Todos os identificadores são gerados pelo serviço após a criação de objetos.

Essa validação não **é um recurso de segurança**. Ele destina-se apenas a informar os aplicativos sobre problemas comuns relacionados ao identificador durante o desenvolvimento do aplicativo, que são difíceis de identificar.


