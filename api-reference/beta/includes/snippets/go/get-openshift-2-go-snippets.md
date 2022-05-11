---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54e9d93800d2ad2193cdaec1060a3fc274fb80d7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322289"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShifts().Get()


```