---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 171ee4e0721fa9d0a9a6b84f7fd9bd29cfecf2a7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323968"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceComplianceId := "managedDeviceCompliance-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagedDeviceCompliancesById(&managedDeviceComplianceId).Get()


```