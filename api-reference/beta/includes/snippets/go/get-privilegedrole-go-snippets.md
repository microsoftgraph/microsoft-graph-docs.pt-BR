---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7607fb66df762576671f3f1eb7640b2139125187
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023691"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

privilegedRoleId := "privilegedRole-id"
result, err := graphClient.PrivilegedRolesById(&privilegedRoleId).Get(options)


```