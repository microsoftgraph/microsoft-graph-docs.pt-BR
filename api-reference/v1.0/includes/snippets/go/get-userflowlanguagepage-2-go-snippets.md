---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c25fcbb1aeb2f7c81e854905ec8438ee957dbcb0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083168"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).OverridesPages().Get(options)


```