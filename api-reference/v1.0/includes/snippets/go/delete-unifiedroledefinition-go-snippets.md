---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c69d2b2123ec14428f1f86f7dfc5b3d4f180924
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285757"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Delete(nil)


```