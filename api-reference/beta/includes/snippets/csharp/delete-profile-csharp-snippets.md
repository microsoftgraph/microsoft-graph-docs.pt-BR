---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b4d82897ee316db64a9828684533a66afa1dd1739657a9f8fde875eb7d87523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile
    .Request()
    .DeleteAsync();

```