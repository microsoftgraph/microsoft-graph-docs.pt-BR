---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9b6184c97b94ce27a923f43cef7286eb1546362
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["contosohr"]
    .Request()
    .DeleteAsync();

```