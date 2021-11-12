---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2412ef23511d711c952299fb37ab6eccf481170b993cac0eda01645ee49c1291
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = await graphClient.Print.Printers["{printer-id}"].TaskTriggers["{printTaskTrigger-id}"]
    .Request()
    .GetAsync();

```