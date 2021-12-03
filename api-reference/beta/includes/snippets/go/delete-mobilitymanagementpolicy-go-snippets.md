---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5fee17f11d29899cc285fc59b223e31c5bf43c9c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286414"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).Delete(nil)


```