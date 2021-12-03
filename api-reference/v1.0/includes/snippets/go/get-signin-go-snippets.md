---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01adfc623deca9817ea8849f8f28bdcc8ed9ba6d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

signInId := "signIn-id"
result, err := graphClient.AuditLogs().SignInsById(&signInId).Get(nil)


```