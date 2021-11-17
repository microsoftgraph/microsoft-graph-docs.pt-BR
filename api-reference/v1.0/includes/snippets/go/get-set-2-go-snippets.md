---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae5bac5c9c4c4bdcb9643f66330b2e07e71650bf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016082"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
setId := "set-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Get(options)


```