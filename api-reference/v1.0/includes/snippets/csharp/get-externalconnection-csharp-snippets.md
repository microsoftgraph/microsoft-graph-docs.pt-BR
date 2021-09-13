---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d90f75947e68989e2fd0aac2ef2a921f48e6f3d16c1576411e72386b4714d170
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = await graphClient.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .GetAsync();

```