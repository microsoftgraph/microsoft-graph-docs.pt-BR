---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 440edfb30023b67701c836f96205f1f1d97defe1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966878"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = new PrintConnector();
printConnector.name = "ConnectorName";
printConnector.fullyQualifiedDomainName = "CONNECTOR-MACHINE";
printConnector.operatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555";
printConnector.appVersion = "0.19.7338.23496";
PrinterLocation location = new PrinterLocation();
location.latitude = 1.1;
location.longitude = 2.2;
location.altitudeInMeters = 3;
printConnector.location = location;

graphClient.print().connectors("{id}")
    .buildRequest()
    .patch(printConnector);

```