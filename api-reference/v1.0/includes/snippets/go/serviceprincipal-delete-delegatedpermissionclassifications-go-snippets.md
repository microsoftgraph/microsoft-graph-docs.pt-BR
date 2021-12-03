---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04bc9a011f795847f9f0b5db09d6e27c3270a1e5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287399"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
delegatedPermissionClassificationId := "delegatedPermissionClassification-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).DelegatedPermissionClassificationsById(&delegatedPermissionClassificationId).Delete(nil)


```