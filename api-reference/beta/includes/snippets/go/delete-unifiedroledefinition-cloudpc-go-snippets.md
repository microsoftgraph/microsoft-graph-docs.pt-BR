---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20535300df05e482d894282d1bf6c370165859b6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
graphClient.RoleManagement().CloudPC().RoleDefinitionsById(&unifiedRoleDefinitionId).Delete()


```