---
title: Tipo de número teamsAsyncOperationType
description: Tipos de teamsAsyncOperation. Os membros serão adicionados aqui à medida que mais operações assíncronas são suportadas.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 8d29e2230dad68c4efbdb5b6bd51a39472de8680
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665806"
---
# <a name="teamsasyncoperationtype-enum-type"></a>Tipo de número teamsAsyncOperationType

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipos de [teamsAsyncOperation](teamsasyncoperation.md). Os membros serão adicionados aqui à medida que mais operações assíncronas são suportadas.

## <a name="members"></a>Members
A tabela a seguir lista os membros de [uma enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Você deve usar o header de solicitação para obter os seguintes valores neste `Prefer: include-unknown-enum-members` número evolvável: `teamifyGroup` , , `createChannel` `createChat` .

| Member | Descrição |
|:---------------|:----------|
|Inválido|Valor inválido.|
|cloneTeam|Operação para clonar uma equipe.|
|archiveTeam|Operação para arquivar uma equipe.|
|unarchiveTeam|Operação para restaurar uma equipe arquivada.|
|createTeam|Operação para criar uma equipe do zero.|
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |
|teamifyGroup |Operação para criar uma equipe de um grupo. |
|createChannel |Operação para criar um canal em uma equipe. |
|createChat|Operação para criar um chat do zero.|
