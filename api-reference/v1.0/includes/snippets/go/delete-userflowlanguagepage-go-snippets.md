---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96941e5b5b1378de71af296821714ce7d87ab6cb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322655"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
userFlowLanguagePageId := "userFlowLanguagePage-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).OverridesPagesById(&userFlowLanguagePageId).$value().Delete()


```