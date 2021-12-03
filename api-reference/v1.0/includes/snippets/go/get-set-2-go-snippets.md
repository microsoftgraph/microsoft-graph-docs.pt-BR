---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bc7ff987b52daf48e7488efbbe4f6b04be94bf8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287050"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
setId := "set-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Get(nil)


```