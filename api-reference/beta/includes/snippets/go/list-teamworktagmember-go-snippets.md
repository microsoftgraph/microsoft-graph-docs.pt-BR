---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc0cda5a4e1cd35d3b83f2e88f547201408e5567
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
result, err := graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Members().Get(options)


```