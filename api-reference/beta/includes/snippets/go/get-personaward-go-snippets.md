---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d37bc15646014c1f0b206b168722acdfce4c03a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090234"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personAwardId := "personAward-id"
result, err := graphClient.Me().Profile().AwardsById(&personAwardId).Get(options)


```