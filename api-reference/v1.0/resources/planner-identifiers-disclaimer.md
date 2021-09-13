---
title: Identificadores no Planner
description: 'Os identificadores de objetos no Planner são valores de cadeia de caracteres gerados pelo serviço. Os valores têm 28 caracteres e são sensíveis a minúsculas. Quando passado como dentro, o serviço fará uma validação de formato simples do identificador, se a validação do formato falhar, os chamadores receberão uma resposta de erro de Solicitação Inossa (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 4433fc63e884f9c98174a07d7d043f69fce4d8c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044417"
---
# <a name="identifiers-in-planner"></a>Identificadores no Planner

Namespace: microsoft.graph

Os identificadores de objetos no Planner são valores de cadeia de caracteres gerados pelo serviço. Os valores têm 28 caracteres e são sensíveis a minúsculas. Quando passado como dentro, o serviço fará uma validação de formato simples do identificador, se a validação do formato falhar, os chamadores receberão uma resposta de erro de Solicitação Inossa (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres sem maiúsculas de minúsculas. Os identificadores em Tarefas são sensíveis a minúsculas.
- O aplicativo de chamada truncado o identificador. Os identificadores em Tarefas têm 28 caracteres.
- O aplicativo de chamada tentou gerar um valor de identificador para um objeto em Tarefas. Identificadores gerados pelo cliente não são aceitos. Todos os identificadores são gerados pelo serviço após a criação de objetos.

Essa validação não **é um recurso de segurança.** Ele só deve informar os aplicativos sobre problemas relacionados ao identificador comum durante o desenvolvimento do aplicativo, que são difíceis de identificar.

