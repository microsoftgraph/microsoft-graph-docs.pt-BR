---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b08fc981865d2aff81497074480cfa7b0b81b301a4e50e3045d5c6102831438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["061b9a92-8926-4bd9-b41d-abf35edc7583"]
    .Close()
    .Request()
    .PostAsync();

```