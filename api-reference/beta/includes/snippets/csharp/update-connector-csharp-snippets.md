---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4842f6ac4d8d6071a07f7ee1aea14ee982d8839
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = new PrintConnector
{
    Name = "ConnectorName",
    FullyQualifiedDomainName = "CONNECTOR-MACHINE",
    OperatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
    AppVersion = "0.19.7338.23496",
    Location = new PrinterLocation
    {
        Latitude = 1.1,
        Longitude = 2.2,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Connectors["{id}"]
    .Request()
    .UpdateAsync(printConnector);

```