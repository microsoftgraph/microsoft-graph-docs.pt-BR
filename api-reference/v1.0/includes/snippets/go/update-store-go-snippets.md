---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51517079b16d640e969b13d215293c48d2d66080
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewStore()
defaultLanguageTag := "en-US"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
siteId := "site-id"
graphClient.SitesById(&siteId).TermStore().Patch(requestBody)


```