---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 493ae2c40ed8bd801df304ac8a6dc9f91da2b343
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286961"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().CloudPC().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(nil)


```