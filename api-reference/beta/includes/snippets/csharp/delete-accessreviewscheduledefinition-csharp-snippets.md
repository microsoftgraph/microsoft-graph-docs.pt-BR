---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 012081787ec3d3668e371a8bc739f8d1f453ec11
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["29f2d16e-9ca6-4052-bbfe-802c48981fd8"]
    .Request()
    .DeleteAsync();

```