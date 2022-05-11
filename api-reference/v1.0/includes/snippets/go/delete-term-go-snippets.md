---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd52c8b05ed9161d38bc8f8973a6032b9e5ac1d6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
setId := "set-id"
termId := "term-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).TermsById(&termId).Delete()


```