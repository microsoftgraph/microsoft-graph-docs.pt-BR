---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 976582f13abd21cfaf79ac30b46ad7bee0b522fe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090177"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
isSyncedFromOnPremises := "Boolean"
requestBody.SetIsSyncedFromOnPremises(&isSyncedFromOnPremises)
options := &msgraphsdk.GetAvailableExtensionPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryObjects().GetAvailableExtensionProperties().Post(options)


```