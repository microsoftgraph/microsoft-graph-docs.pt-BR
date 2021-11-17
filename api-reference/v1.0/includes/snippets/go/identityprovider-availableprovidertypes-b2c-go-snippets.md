---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a19868a48a88ef64a958ea39ee84a4b94fd6058c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019030"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Get(options)


```