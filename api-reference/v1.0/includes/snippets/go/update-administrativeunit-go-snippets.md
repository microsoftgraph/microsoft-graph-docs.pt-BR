---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2475801aa6f2d508dd96b5ef9482c3f49913f932
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322972"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAdministrativeUnit()
displayName := "Greater Seattle District Technical Schools"
requestBody.SetDisplayName(&displayName)
administrativeUnitId := "administrativeUnit-id"
graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).Patch(requestBody)


```