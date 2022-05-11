---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 233d1efc2cc51c6e23bf67490da0dddf5e6fbd6c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324350"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSecurityEnabledOnlyRequestBody()
securityEnabledOnly := false
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly)
directoryObjectId := "directoryObject-id"
result, err := graphClient.DirectoryObjectsById(&directoryObjectId).GetMemberGroups(directoryObject-id).Post(requestBody)


```