---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e00cfed1b38798ce525a88501615d843f4aac8bb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031658"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).PermissionGrants().Get(options)


```