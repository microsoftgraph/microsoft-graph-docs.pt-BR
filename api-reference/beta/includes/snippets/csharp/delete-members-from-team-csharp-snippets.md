---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f051fc80c08d842b3d7ea5810ae0686be2c8b6c
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamsId}"].Members
    .Request()
    .DeleteAsync();

```