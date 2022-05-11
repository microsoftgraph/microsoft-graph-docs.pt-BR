---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc99a324cbbcfa7bbd010a3d50a9c5bb44b4590a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324065"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantId := "tenant-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsById(&tenantId).ResetTenantOnboardingStatus(tenant-id).Post()


```