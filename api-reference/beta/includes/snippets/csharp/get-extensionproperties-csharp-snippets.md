---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0198f2abb444a6bb9047b0a556dd90833c920bab
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995447"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensionProperties = await graphClient.Applications["{id}"].ExtensionProperties
    .Request()
    .GetAsync();

```