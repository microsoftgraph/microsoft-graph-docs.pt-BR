---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e75baa1cee41ce68d17a558af8f73df8164ea2b7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324928"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceComplianceTrendId := "managedDeviceComplianceTrend-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagedDeviceComplianceTrendsById(&managedDeviceComplianceTrendId).Get()


```