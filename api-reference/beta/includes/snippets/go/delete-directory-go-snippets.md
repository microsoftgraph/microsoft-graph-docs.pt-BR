---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4813804e262710eaefb44038c4eb13c5ce6f2ee8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryObjectId := "directoryObject-id"
graphClient.Directory().DeletedItemsById(&directoryObjectId).Delete()


```