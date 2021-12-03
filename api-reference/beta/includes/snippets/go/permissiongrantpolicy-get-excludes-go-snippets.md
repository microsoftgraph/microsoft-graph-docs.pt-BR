---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44c347cb3efa812acd7d1647acadedb37a93e7f3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287360"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Excludes().Get(nil)


```