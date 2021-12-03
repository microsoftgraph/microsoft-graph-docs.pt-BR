---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0c362af4c79c34ab610ab6c23e8feee0516c116
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
result, err := graphClient.SitesById(&siteId).TermStore().Get(nil)


```