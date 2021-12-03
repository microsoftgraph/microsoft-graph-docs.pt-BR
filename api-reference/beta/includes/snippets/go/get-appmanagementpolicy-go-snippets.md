---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 943fba68b4869ea62b42dc00777a6fca82f067f4
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285811"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

appManagementPolicyId := "appManagementPolicy-id"
result, err := graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).Get(nil)


```