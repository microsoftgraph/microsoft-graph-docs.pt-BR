---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a01e33e4b4ef16c6d123b087e546d745f84c34e4
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286788"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedApprovalId := "privilegedApproval-id"
result, err := graphClient.PrivilegedApprovalById(&privilegedApprovalId).Get(nil)


```