---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afc47e59e5d5705ea1db655e1ce51abc5e07cade
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002705"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityProviderBaseId := "identityProviderBase-id"
graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Delete(options)


```