---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19c6358f1fc46917b25ff249e33431a5ee5efc31
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325001"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
userFlowLanguagePageId := "userFlowLanguagePage-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).DefaultPagesById(&userFlowLanguagePageId).$value().Get()


```