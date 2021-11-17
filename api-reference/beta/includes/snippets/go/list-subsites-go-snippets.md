---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 721fc14e173359964924796098e93aebbdd4db21
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020463"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Sites().Get(options)


```