---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28b5620f17c34a98d8cac02be07966d719797b5d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287115"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Oauth2PermissionGrants().Get(nil)


```