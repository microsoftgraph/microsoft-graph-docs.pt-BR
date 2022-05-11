---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1c734c91fa158502d6b355bf4c9d053f01250aa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325123"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactId := "contact-id"
result, err := graphClient.Me().ContactsById(&contactId).Get()


```