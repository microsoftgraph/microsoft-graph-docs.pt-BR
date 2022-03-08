---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1fc3138ba290e7c3ecbc6478eae9731b519d7cd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338433"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

acronymId := "acronym-id"
graphClient.Search().AcronymsById(&acronymId).Delete(nil)


```