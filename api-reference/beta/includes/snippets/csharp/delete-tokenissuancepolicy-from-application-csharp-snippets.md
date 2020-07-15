---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41447be03cfb16602373ef199db72493f02e2d37
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].TokenIssuancePolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```