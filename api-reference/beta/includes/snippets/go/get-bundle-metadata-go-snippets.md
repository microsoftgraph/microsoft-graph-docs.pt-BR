---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04140b0f63f155e8a70c4831a788a4fa82779dab
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324901"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
result, err := graphClient.Drive().BundlesById(&driveItemId).Get()


```