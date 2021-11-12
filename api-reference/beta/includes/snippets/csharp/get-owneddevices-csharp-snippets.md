---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52e4e332a3cea354213110db40cf3e534964f329d9c33d8072e9f35203cff32a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375880"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedDevices = await graphClient.Me.OwnedDevices
    .Request()
    .GetAsync();

```