---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 330fe616d7dcdde1e43e382c1909c75a8c75e294
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
groupId := "group-id"
result, err := graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Sets().Get(nil)


```