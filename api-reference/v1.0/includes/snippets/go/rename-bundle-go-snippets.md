---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d6f377dc06be91d79131f73f86f0a485051a466
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323521"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDriveItem()
name := "Shared legal agreements"
requestBody.SetName(&name)
driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Patch(requestBody)


```