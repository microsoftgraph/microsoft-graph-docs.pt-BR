---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0528e21c4a907af237473740b3834568352d44c7e4b03066913762ae46bb94e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publications = await graphClient.Me.Profile.Publications
    .Request()
    .GetAsync();

```