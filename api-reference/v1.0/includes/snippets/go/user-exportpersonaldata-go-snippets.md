---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c607abbe7a8a5f8a33b78482f25d874f11ce9ee3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324171"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewStorageLocationRequestBody()
storageLocation := "storageLocation-value"
requestBody.SetStorageLocation(&storageLocation)
userId := "user-id"
graphClient.UsersById(&userId).ExportPersonalData(user-id).Post(requestBody)


```