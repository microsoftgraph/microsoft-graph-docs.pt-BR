---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26843b1aca2a1ecbb34f5ffd31140eab26aeaa71
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002117"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
permissionId := "permission-id"
result, err := graphClient.SitesById(&siteId).PermissionsById(&permissionId).Get(options)


```