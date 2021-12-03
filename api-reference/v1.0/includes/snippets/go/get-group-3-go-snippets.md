---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 260d068f032a0c221e8fddb6d39c7d2959dc9050
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286457"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
groupId := "group-id"
result, err := graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Get(nil)


```