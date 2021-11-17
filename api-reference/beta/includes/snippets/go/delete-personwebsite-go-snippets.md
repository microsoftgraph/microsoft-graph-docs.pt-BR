---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 868d16c693fa1f9593018abf3fcdd40e71215923
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personWebsiteId := "personWebsite-id"
graphClient.Me().Profile().WebsitesById(&personWebsiteId).Delete(options)


```