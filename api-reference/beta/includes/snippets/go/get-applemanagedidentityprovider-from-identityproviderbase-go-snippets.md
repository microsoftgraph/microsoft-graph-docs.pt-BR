---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b60fa8325e386f8d62aa5afe536fc70d1b29882e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098222"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Get(options)


```