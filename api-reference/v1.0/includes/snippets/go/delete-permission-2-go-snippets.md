---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ac31cedd873099d50ebefc4b03784973214bf38
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287397"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
permissionId := "permission-id"
graphClient.SitesById(&siteId).PermissionsById(&permissionId).Delete(nil)


```