---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c67af0eefd1b5b8219999d68d773d8d47f1e475c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100709"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).GroupLifecyclePolicies().Get(options)


```