---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02fa275cb4c9306d0ef4579b608240af1b828a72
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryObjectId := "directoryObject-id"
graphClient.Directory().DeletedItemsById(&directoryObjectId).Delete(nil)


```