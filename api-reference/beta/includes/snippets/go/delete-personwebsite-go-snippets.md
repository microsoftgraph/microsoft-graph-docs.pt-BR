---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe1de906c1dc35a0d17c0f13ab2103d7f7fe8152
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personWebsiteId := "personWebsite-id"
graphClient.Me().Profile().WebsitesById(&personWebsiteId).Delete(options)


```