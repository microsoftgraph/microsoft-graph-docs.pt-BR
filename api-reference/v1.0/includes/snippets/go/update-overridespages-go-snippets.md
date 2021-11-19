---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7a08c13ffb32220f681fa11327b1c12f06a9a90
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098416"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "LocalizedStrings":  []Object {
    }
}
options := &msgraphsdk.ContentRequestBuilderPutOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
userFlowLanguagePageId := "userFlowLanguagePage-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).OverridesPagesById(&userFlowLanguagePageId).$value().Put(options)


```