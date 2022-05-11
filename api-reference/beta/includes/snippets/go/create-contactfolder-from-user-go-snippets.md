---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0940325cfac4f5dae58171b0b5c9b5695be28ed2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325324"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactFolder()
parentFolderId := "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=="
requestBody.SetParentFolderId(&parentFolderId)
displayName := "Important contacts"
requestBody.SetDisplayName(&displayName)
result, err := graphClient.Me().ContactFolders().Post(requestBody)


```