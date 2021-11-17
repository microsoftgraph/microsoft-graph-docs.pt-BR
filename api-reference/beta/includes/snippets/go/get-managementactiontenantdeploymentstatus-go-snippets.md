---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ab9e0756f17a2ab9f25c4c8dd338b1616ecff26
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011903"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

managementActionTenantDeploymentStatusId := "managementActionTenantDeploymentStatus-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionTenantDeploymentStatusesById(&managementActionTenantDeploymentStatusId).Get(options)


```