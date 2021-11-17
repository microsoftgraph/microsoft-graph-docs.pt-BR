---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51e4ba3a61c53c5cedc8c1fa496f19f905f69c9a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976871"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

trustFrameworkPolicyId := "trustFrameworkPolicy-id"
graphClient.TrustFramework().PoliciesById(&trustFrameworkPolicyId).Delete(options)


```