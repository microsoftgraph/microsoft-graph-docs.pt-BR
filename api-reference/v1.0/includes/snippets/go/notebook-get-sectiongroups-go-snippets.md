---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de5b2a26b4c459717792a0d2ea7fc03f8991f526
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).SectionGroups().Get(nil)


```