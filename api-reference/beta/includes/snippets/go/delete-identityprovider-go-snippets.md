---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9be3df31a40843a69c11163f71d23ece8b0d7aa7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015046"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Delete(options)


```