---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6faa2c054d0e991e4f1bdf33c6a60c15bacf5b39
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324080"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
contentTypeId := "contentType-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).IsPublished()(site-id, contentType-id).Get()


```