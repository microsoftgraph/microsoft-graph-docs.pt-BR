---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18f36f79d72c2001af2d4067a515b50c24bfe78b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286379"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Get(nil)


```