---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c72ddd1b2c6a11bcd19df54eb51134bfc5deb4a92092089d24b7bfa2f70762eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329490"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{event-id}"].Attachments["{attachment-id}"]
    .Request()
    .DeleteAsync();

```