---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95f0e7ef78291830e4ca5477367528168c78a5f1
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286474"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
permissionId := "permission-id"
result, err := graphClient.SitesById(&siteId).PermissionsById(&permissionId).Get(nil)


```