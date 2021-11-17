---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f575d8f0dfcb5feea20e61e1ec3ea660c454a11f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988403"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
setId := "set-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Delete(options)


```