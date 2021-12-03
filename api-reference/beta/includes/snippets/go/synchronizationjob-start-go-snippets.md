---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0286bef40b9b748a6c03d8c5b7021c656500c5c7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287385"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Start().Post(nil)


```