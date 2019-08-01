---
title: Identificadores no Planner
description: 'Os identificadores para objetos no Planner são valores de cadeia de caracteres gerados pelo serviço. Os valores têm 28 caracteres de comprimento e diferenciam maiúsculas de minúsculas. Quando transmitido como em, o serviço fará uma validação de formato simples do identificador, se a validação de formato falhar, os chamadores receberão uma resposta de erro de solicitação inválida (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 75a0262b085b6649d7390a2a6196d0190cdefc5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035445"
---
# <a name="identifiers-in-planner"></a>Identificadores no Planner

Os identificadores para objetos no Planner são valores de cadeia de caracteres gerados pelo serviço. Os valores têm 28 caracteres de comprimento e diferenciam maiúsculas de minúsculas. Quando transmitido como em, o serviço fará uma validação de formato simples do identificador, se a validação de formato falhar, os chamadores receberão uma resposta de erro de solicitação inválida (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres não sensível a um caso. Os identificadores nas tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncava o identificador. Os identificadores nas tarefas têm 28 caracteres de comprimento.
- O aplicativo de chamada tentou gerar um valor de identificador para um objeto nas tarefas. Os identificadores gerados pelo cliente não são aceitos. Todos os identificadores são gerados pelo serviço na criação de objetos.

Essa validação **não é um recurso de segurança**. O objetivo é apenas informar aplicativos sobre problemas relacionados ao identificador comum durante o desenvolvimento do aplicativo, o que, de outra forma, é difícil de identificar.
