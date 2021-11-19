---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48da19c82b0e34260853e38e552dde8d37242083
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101699"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceComplianceTrendId := "managedDeviceComplianceTrend-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagedDeviceComplianceTrendsById(&managedDeviceComplianceTrendId).Get(options)


```