---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efdbef8d4b5d99416d51c3bb64b95c750bbf8a4e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325168"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionTenantDeploymentStatuses().ChangeDeploymentStatus().Post(requestBody)


```