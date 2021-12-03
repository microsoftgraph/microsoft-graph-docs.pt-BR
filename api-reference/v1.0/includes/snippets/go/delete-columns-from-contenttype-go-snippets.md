---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ce4ba83bf8ea5115fafd6cd7a3de9f55bebde52
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287268"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
contentTypeId := "contentType-id"
columnDefinitionId := "columnDefinition-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).ColumnsById(&columnDefinitionId).Delete(nil)


```