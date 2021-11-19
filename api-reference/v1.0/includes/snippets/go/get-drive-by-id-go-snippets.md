---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75ae8c636ab9f533a6138c10390ea0da8cc0b405
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095724"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
result, err := graphClient.DrivesById(&driveId).Get(options)


```