---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4646d836d687888a80fb9d402b26550ee6b043e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323619"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Get()


```