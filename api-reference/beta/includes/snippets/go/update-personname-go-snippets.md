---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61b2ee3433f04f8a55a20d2f51cd6ec7b78bf7c5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323874"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonName()
nickname := "Kesha"
requestBody.SetNickname(&nickname)
personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Patch(requestBody)


```