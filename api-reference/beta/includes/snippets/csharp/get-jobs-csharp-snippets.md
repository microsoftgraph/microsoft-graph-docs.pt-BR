---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd870a73fad166f2b428adae18352f654c9e7a3d
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.Print.Shares["{id}"].Jobs
    .Request()
    .GetAsync();

```