---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94af1324b90fe0e14e0152df7c02d4a55a805a94960c231deecc9d93a1b7f223
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{drive-id}"]
    .Request()
    .GetAsync();

```