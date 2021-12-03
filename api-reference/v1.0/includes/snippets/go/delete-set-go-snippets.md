---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 458b5bb46ecdf7b86470bf129f73676b26cf43d3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
setId := "set-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Delete(nil)


```