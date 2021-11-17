---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb1290f1b4488b019525800966cf2e73067de390
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011889"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

managementTemplateId := "managementTemplate-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementTemplatesById(&managementTemplateId).Get(options)


```