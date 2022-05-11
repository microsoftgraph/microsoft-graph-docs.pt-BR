---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9552be20a6c38cd386496ba5a1b5984c03b32cd0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitionsById(&unifiedRoleDefinitionId).Get()


```