---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76c4da0d9d30f78d6d76228cd47ec84d6ef9198a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095636"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
graphClient.TermStore().SetsById(&setId).Delete(options)


```