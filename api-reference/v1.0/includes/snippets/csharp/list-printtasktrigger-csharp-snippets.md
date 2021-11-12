---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a66b6b956bed4b3c34a1babfba48c2802f3a97eee32e28623d6ce9bac8ccee4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273102"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskTriggers = await graphClient.Print.Printers["{printer-id}"].TaskTriggers
    .Request()
    .GetAsync();

```