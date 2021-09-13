---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11a2d1a692ac6d5dc80126e01508bdee81d5797b415c5357f32527752c955d2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214950"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rooms = await graphClient.Places["{place-id}"].Rooms
    .Request()
    .GetAsync();

```