---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07a9565e68d831e9f1fa72ee3c3f2605453f24267699f27f1ffa108a81d5d410
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealthIssue = await graphClient.Admin.ServiceAnnouncement.Issues["{serviceHealthIssue-id}"]
    .Request()
    .GetAsync();

```