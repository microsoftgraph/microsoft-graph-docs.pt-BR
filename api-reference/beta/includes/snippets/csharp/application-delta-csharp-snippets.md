---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27d4d16fd8274074e7c89d54879085a3f97a8be5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855299"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Applications
    .Delta()
    .Request()
    .GetAsync();

```