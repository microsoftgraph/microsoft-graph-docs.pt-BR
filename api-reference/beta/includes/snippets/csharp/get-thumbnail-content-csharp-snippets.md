---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adfa45220ecfcff0b737460c6b5aade86162f143a88f9f74221cc7ba283bdc6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails["{thumbnailSet-id}"]["{thumbnailSet-id}"].Content
    .Request()
    .GetAsync();

```