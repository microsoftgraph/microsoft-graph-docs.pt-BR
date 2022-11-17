---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84519a1664b1ad371424ac9b64332363ab1f46e5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994696"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Delete(options)


```