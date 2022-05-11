---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23e4d792c2ed44252ad67381584f398e9feb284e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322264"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWorkPosition()
isCurrent := true
requestBody.SetIsCurrent(&isCurrent)
workPositionId := "workPosition-id"
graphClient.Me().Profile().PositionsById(&workPositionId).Patch(requestBody)


```