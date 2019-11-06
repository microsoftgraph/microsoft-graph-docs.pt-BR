---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 986ea2e159fdc3c9522d6ffada370147451a19ed
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = await graphClient.Connections["contosohr"]
    .Request()
    .GetAsync();

```