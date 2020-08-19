---
title: Identificadores nas tarefas
description: 'Os identificadores para objetos nas tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores têm 28 caracteres de comprimento e diferenciam maiúsculas de minúsculas. Quando transmitido como em, o serviço fará uma validação de formato simples do identificador, se a validação de formato falhar, os chamadores receberão uma resposta de erro de solicitação inválida (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:'
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: TarkanSevilmis
ms.openlocfilehash: 9ff7b894c8414e2dc7f3dd9d425b0027d0ae13f5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811956"
---
# <a name="identifiers-in-tasks"></a>Identificadores nas tarefas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os identificadores para objetos nas tarefas são valores de cadeia de caracteres gerados pelo serviço. . Os valores têm 28 caracteres de comprimento e diferenciam maiúsculas de minúsculas. Quando transmitido como em, o serviço fará uma validação de formato simples do identificador, se a validação de formato falhar, os chamadores receberão uma resposta de erro de solicitação inválida (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres não sensível a um caso. Os identificadores nas tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncava o identificador. Os identificadores nas tarefas têm 28 caracteres de comprimento.
- O aplicativo de chamada tentou gerar um valor de identificador para um objeto nas tarefas. Os identificadores gerados pelo cliente não são aceitos. Todos os identificadores são gerados pelo serviço na criação de objetos.

Essa validação **não é um recurso de segurança**. O objetivo é apenas informar aplicativos sobre problemas relacionados ao identificador comum durante o desenvolvimento do aplicativo, o que, de outra forma, é difícil de identificar.
