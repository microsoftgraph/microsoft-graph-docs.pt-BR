---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc71e0471685e03f81d040c382112b4bb207c43c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094961"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Delete(options)


```