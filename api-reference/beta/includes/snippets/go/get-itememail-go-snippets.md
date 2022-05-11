---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b70edc7c08e2ecdd06f3a8cbdbc080ba4dbf5bc7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324274"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemEmailId := "itemEmail-id"
result, err := graphClient.UsersById(&userId).Profile().EmailsById(&itemEmailId).Get()


```