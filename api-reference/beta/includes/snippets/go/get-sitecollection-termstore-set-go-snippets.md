---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37c7cab66810b066ebaff144e941a88684ee6b89
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325687"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
setId := "set-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Get()


```