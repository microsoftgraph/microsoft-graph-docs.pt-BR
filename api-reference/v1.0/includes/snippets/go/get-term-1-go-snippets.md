---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64b530005d391cb045d078872bf2aa469fa32265
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
groupId := "group-id"
setId := "set-id"
termId := "term-id"
result, err := graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).SetsById(&setId).TermsById(&termId).Get(options)


```