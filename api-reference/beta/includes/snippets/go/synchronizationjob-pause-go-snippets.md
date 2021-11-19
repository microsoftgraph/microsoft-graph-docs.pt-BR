---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 574f0bf223d1d32f691e6cc7ad53cab3a970cb46
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093587"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Pause().Post(options)


```