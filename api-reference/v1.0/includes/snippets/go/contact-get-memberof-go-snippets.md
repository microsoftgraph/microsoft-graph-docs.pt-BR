---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7481efc7ade9951dc55206f234c198c0cb49eeca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).MemberOf().Get(options)


```