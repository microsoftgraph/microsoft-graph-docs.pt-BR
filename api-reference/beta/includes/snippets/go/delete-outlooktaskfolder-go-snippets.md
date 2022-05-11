---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62ad1a85782d3212ba4e6bffb76dada2e34ada60
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323876"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookTaskFolderId := "outlookTaskFolder-id"
graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Delete()


```