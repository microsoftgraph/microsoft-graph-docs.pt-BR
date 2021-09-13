---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b66f5b84dc13e4049b21ee687bc08fcb12ad5ff775e830d1ffe0412ef95ebb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Special["{driveItem-id}"]
    .Request()
    .GetAsync();

```