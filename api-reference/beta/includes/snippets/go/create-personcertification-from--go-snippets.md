---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7fee147ee2a79a287dbe87bcc1c74d65df33ff7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027933"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonCertification()
certificationId := "KB-1235466333663322"
requestBody.SetCertificationId(&certificationId)
description := "Blackbelt in Marketing - Brand Management"
requestBody.SetDescription(&description)
displayName := "Marketing Blackbelt - Brand Management"
requestBody.SetDisplayName(&displayName)
thumbnailUrl := "https://iame.io/dfhdfdfd334.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
webUrl := "https://www.iame.io/blackbelt"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.CertificationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Certifications().Post(options)


```