---
title: tipo de enumeração teamsAsyncOperationStatus
description: Descreve o status atual de um teamsAsyncOperation.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c82065c789847d3e2a11947dcf921b12c55530e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519894"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>tipo de enumeração teamsAsyncOperationStatus

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status atual de um [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Inválido|,0|Valor inválido.|
|notStarted|1 |A operação não foi iniciada.|
|inProgress|2 |A operação está sendo executada.|
|adicionada|3 |A operação foi bem-sucedida.|
|falhou|4 |Falha na operação.|
