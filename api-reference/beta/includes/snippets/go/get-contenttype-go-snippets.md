---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54e67ca47c237931d2b5843f2017abb069dc54a4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028739"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
contentTypeId := "contentType-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Get(options)


```