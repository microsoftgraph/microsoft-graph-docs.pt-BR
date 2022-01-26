---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 059ede741581127132027d3f29ac21653eccc03f
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225081"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
userAccountType := "administrator"
requestBody.SetUserAccountType(&userAccountType)
osVersion := "windows10"
requestBody.SetOsVersion(&osVersion)
options := &msgraphsdk.ReprovisionRequestBuilderPostOptions{
    Body: requestBody,
}
cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).Reprovision().Post(options)


```