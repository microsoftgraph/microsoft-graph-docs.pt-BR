---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac20bac5a99f95816154577c79547ae572d6442a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022048"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
tenantGroupId := "String"
requestBody.SetTenantGroupId(&tenantGroupId)
tenantId := "String"
requestBody.SetTenantId(&tenantId)
managementActionId := "String"
requestBody.SetManagementActionId(&managementActionId)
managementTemplateId := "String"
requestBody.SetManagementTemplateId(&managementTemplateId)
status := "String"
requestBody.SetStatus(&status)
options := &msgraphsdk.ChangeDeploymentStatusRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionTenantDeploymentStatuses().ChangeDeploymentStatus().Post(options)


```