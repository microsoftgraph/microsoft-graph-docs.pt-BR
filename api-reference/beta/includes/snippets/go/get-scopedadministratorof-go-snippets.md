---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6abf832670e24dde2029477b8d5a7d40288a383f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().ScopedRoleMemberOf().Get(options)


```