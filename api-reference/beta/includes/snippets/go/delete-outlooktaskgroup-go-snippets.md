---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 900ab6bb8c881d38092b038d1f193fb2eadf0239
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287101"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookTaskGroupId := "outlookTaskGroup-id"
graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).Delete(nil)


```