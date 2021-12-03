---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1a6b57af10e4b19ea3bd5125d633170cca025c6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
result, err := graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).Get(nil)


```