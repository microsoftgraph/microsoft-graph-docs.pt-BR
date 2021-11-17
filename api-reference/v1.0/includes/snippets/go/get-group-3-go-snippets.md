---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71e2cf03d32965e9588d6b044145468fdd53a075
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
groupId := "group-id"
result, err := graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Get(options)


```