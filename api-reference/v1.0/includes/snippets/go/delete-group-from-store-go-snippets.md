---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b72ab209d545ebf57630dd45bf26f9d32b97dd9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087015"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
groupId := "group-id"
graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Delete(options)


```