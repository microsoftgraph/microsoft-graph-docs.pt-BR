---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b426fb226ad2cb8bfc6d0dc45af1a23c53cd40a0
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).Renew().Post(nil)


```