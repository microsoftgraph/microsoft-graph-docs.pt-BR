---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bb9843902566458696a663822d85545065cf000
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020716"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcDeviceId := "cloudPcDevice-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcDevicesById(&cloudPcDeviceId).Get(options)


```