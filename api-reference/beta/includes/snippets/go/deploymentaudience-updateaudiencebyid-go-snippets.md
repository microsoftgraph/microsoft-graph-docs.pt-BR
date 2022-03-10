---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7bdab078da102bb20dc96749234987fee129a0d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410871"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
memberEntityType := "String"
requestBody.SetMemberEntityType(&memberEntityType)
requestBody.SetAddMembers( []String {
    "String",
}
requestBody.SetRemoveMembers( []String {
    "String",
}
requestBody.SetAddExclusions( []String {
    "String",
}
requestBody.SetRemoveExclusions( []String {
    "String",
}
options := &msgraphsdk.UpdateAudienceByIdRequestBuilderPostOptions{
    Body: requestBody,
}
deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Audience().UpdateAudienceById(deployment-id).Post(options)


```