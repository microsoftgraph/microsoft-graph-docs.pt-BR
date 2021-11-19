---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3004b8afd05b7180bf899cb86970b24575c9603
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093562"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
graphClient.UsersById(&userId).Delete(options)


```