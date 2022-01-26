---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdf58c7d8d8dc77de4add86028b0539f6fbce6bb
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62227507"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).TaughtClasses().Get(nil)


```