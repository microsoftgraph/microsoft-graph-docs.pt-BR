---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8078059738f17160b28e6fc6137d29256f08600e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
contentTypeId := "contentType-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Get()


```