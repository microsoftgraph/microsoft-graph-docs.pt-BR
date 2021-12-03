---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e927934e133adc54b6cc48bd14a02980be33db8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286144"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Get(nil)


```