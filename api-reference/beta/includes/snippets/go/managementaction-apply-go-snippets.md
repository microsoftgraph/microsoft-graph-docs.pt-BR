---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83b70aa19006b511aab81f86e2257ebc6b91a917
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324835"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
tenantGroupId := "String"
requestBody.SetTenantGroupId(&tenantGroupId)
managementTemplateId := "String"
requestBody.SetManagementTemplateId(&managementTemplateId)
managementActionId := "managementAction-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionsById(&managementActionId).Apply(managementAction-id).Post(requestBody)


```