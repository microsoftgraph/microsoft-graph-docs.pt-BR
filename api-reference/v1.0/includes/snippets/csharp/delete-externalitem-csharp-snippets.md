---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35fe3b50fa730ab83a4f6cb7d558b8e0d789a4c8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .DeleteAsync();

```