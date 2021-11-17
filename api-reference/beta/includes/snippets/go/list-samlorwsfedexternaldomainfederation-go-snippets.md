---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e85f47e234d42b2fafa38430b252216b4edde16
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979925"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Get(options)


```