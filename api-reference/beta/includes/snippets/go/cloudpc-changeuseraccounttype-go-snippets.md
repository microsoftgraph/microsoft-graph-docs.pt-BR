---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 433aa3db2830a3fd8ecf0c8efc7b350a86d69164
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411030"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountTypeRequestBody()
userAccountType := "administrator"
requestBody.SetUserAccountType(&userAccountType)
options := &msgraphsdk.ChangeUserAccountTypeRequestBuilderPostOptions{
    Body: requestBody,
}
cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).ChangeUserAccountType(cloudPC-id).Post(options)


```