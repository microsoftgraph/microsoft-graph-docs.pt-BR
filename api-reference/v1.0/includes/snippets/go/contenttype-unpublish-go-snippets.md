---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89f8a4ccfa068d9895c32913a298d9aa11ed3547
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285776"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
contentTypeId := "contentType-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Unpublish().Post(nil)


```