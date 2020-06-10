---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca18208068f36d4cf8940385a83b80b558cf4d82
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = new Printer
{
    Name = "PrinterName",
    Location = new PrinterLocation
    {
        Latitude = 1.1f,
        Longitude = 2.2f,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Printers["{id}"]
    .Request()
    .UpdateAsync(printer);

```