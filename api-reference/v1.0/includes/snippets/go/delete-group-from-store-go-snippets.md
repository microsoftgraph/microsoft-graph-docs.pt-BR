---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79104c94389bc75f96655326a465bab65094b5ee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008662"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
groupId := "group-id"
graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Delete(options)


```