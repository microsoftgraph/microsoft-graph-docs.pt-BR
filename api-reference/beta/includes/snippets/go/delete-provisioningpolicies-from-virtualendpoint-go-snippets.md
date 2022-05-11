---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 724ecfcbbb83245d4637aa34ca192a9bb4d8d1cc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324081"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Delete()


```