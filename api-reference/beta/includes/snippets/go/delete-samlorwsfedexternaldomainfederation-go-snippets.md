---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23fee6affd7c58676b61d2ad0faf119dc1029c57
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderBaseId := "identityProviderBase-id"
graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Delete(options)


```