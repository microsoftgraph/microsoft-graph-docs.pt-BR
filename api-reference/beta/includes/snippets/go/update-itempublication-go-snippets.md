---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f957b58f18bfb10075fe73bcafaf0941d1b6caa
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286336"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemPublicationId := "itemPublication-id"
graphClient.UsersById(&userId).Profile().PublicationsById(&itemPublicationId).Patch(nil)


```