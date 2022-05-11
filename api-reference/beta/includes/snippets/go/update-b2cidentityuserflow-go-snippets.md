---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 863d47eee0fb548d306ad585077244fca0f1d85c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324706"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2cIdentityUserFlow()
isLanguageCustomizationEnabled := true
requestBody.SetIsLanguageCustomizationEnabled(&isLanguageCustomizationEnabled)
defaultLanguageTag := "en"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Patch(requestBody)


```