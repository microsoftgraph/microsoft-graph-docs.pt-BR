---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db0975e347a1c1c07d69e168a9d340d81fd1553000b779a9f57ecf88b1844f5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Schema
    .Request()
    .GetAsync();

```