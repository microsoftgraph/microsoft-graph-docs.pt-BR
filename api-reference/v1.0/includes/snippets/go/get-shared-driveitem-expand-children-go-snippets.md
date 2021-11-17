---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 891fa27d371c9102e2ce690c9f6b81c4486611ef
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012892"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DriveItemRequestBuilderGetQueryParameters{
    Expand: "children",
}
options := &msgraphsdk.DriveItemRequestBuilderGetOptions{
    Q: requestParameters,
}
sharedDriveItemId := "sharedDriveItem-id"
result, err := graphClient.SharesById(&sharedDriveItemId).DriveItem().Get(options)


```