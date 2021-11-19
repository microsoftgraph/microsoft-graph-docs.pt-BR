---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a25e6804c89ff2a5d20baa12ee9c864b16e6ff11
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092997"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
shiftId := "shift-id"
result, err := graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Get(options)


```