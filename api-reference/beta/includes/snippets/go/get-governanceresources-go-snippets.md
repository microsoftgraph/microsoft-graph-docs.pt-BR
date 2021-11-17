---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 488fd4a2fe5589b45156dc20489f096aa8a2d878
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020897"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).Resources().Get(options)


```