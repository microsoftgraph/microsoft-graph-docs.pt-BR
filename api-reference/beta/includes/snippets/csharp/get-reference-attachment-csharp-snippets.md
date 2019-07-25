---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bb5f3e008250e82da1e3fa72f2e6c2c07b06660
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710228"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Events["AAMkAGE1M88AADUv0uAAAG="].Attachments["AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
    .Request()
    .GetAsync();

```