---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9362d9b4a81205047fc45ae84c730392b6b9b9b6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287033"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookTaskFolderId := "outlookTaskFolder-id"
result, err := graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Get(nil)


```