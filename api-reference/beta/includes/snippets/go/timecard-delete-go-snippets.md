---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2303217922ad829acf3412e1df64e598cb01384
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101623"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeCardId := "timeCard-id"
graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).Delete(options)


```