---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b797523f5bd8b20faaf589ecaa45892d2a227907
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
    .Request()
    .GetAsync();

```