---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3ab265bcb73d545bd10eebf08788a1096a788b9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325308"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
setId := "set-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Delete()


```