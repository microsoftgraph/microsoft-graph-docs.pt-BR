---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 277c52dd7fc592ffb6cc2ce5ab36d8c87d47e722
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325539"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).TransitiveMembers().Get()


```