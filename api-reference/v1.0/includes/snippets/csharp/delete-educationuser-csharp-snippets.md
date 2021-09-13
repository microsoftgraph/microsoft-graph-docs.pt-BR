---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df36bb5cbeaaea72454eab3007cefc19e2bb4c3f4c61a6489917d5ffb955a34c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328083"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```