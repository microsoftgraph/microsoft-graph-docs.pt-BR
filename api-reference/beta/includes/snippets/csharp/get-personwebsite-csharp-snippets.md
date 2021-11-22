---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bf7da90614886ed781b931defda4060a218f27f51a82cbe0460998432032e34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = await graphClient.Me.Profile.Websites["{personWebsite-id}"]
    .Request()
    .GetAsync();

```