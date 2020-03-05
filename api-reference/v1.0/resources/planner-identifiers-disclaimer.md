---
title: Identificadores no Planner
description: 'Os identificadores para objetos no Planner são valores de cadeia de caracteres gerados pelo serviço. Os valores têm 28 caracteres de comprimento e diferenciam maiúsculas de minúsculas. Quando transmitido como em, o serviço fará uma validação de formato simples do identificador, se a validação de formato falhar, os chamadores receberão uma resposta de erro de solicitação inválida (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 32d00a6e93d09287087ee52bc024519828f7e822
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447168"
---
# <a name="identifiers-in-planner"></a>Identificadores no Planner

Namespace: Microsoft. Graph

Os identificadores para objetos no Planner são valores de cadeia de caracteres gerados pelo serviço. Os valores têm 28 caracteres de comprimento e diferenciam maiúsculas de minúsculas. Quando transmitido como em, o serviço fará uma validação de formato simples do identificador, se a validação de formato falhar, os chamadores receberão uma resposta de erro de solicitação inválida (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres não sensível a um caso. Os identificadores nas tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncava o identificador. Os identificadores nas tarefas têm 28 caracteres de comprimento.
- O aplicativo de chamada tentou gerar um valor de identificador para um objeto nas tarefas. Os identificadores gerados pelo cliente não são aceitos. Todos os identificadores são gerados pelo serviço na criação de objetos.

Essa validação **não é um recurso de segurança**. O objetivo é apenas informar aplicativos sobre problemas relacionados ao identificador comum durante o desenvolvimento do aplicativo, o que, de outra forma, é difícil de identificar.
