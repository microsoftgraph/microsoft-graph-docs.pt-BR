---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea78a3f9c810a6e8d5100d90d6e3cd4313527845675b7f92171310f9b86d46a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Domains
    .Request()
    .GetAsync();

```