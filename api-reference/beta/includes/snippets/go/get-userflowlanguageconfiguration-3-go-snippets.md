---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4542e6828cc53384791a64ea6d2d3be35d939997
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286033"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).Get(nil)


```