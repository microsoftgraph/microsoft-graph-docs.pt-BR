---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52f81bee946bee404f0deb8be3ce378bb158ef47
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097939"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
permissionId := "permission-id"
result, err := graphClient.SitesById(&siteId).PermissionsById(&permissionId).Get(options)


```