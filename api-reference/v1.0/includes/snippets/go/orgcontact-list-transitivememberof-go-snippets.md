---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5fba39abffcb58280e38368f111a04e2c98a20d2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322234"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).TransitiveMemberOf().Get()


```