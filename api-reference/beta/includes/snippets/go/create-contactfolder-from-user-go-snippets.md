---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9a7acccf91e1d07276c1c71460cdf78056cfebc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091551"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactFolder()
parentFolderId := "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=="
requestBody.SetParentFolderId(&parentFolderId)
displayName := "Important contacts"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ContactFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().ContactFolders().Post(options)


```