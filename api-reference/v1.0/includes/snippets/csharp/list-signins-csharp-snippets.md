---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 961b3a609b2cc3cecd6279d980bb73f7c187f652bd47d80a4c1610a104bcb4e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIns = await graphClient.AuditLogs.SignIns
    .Request()
    .GetAsync();

```