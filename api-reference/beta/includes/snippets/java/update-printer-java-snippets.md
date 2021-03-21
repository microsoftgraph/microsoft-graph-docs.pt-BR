---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66f5eaf8e7d58cca522df824d90a3acfeacba9ed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = new Printer();
printer.name = "PrinterName";
PrinterLocation location = new PrinterLocation();
location.latitude = 1.1d;
location.longitude = 2.2d;
location.altitudeInMeters = 3;
printer.location = location;

graphClient.print().printers("{id}")
    .buildRequest()
    .patch(printer);

```