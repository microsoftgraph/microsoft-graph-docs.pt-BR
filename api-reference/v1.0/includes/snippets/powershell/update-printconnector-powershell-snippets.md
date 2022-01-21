---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a757016b581bc509cc1f1be6353b084f10047012
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116980"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    DisplayName = "ConnectorName"
    FullyQualifiedDomainName = "CONNECTOR-MACHINE"
    OperatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555"
    AppVersion = "0.19.7338.23496"
    Location = @{
        Latitude = 1.1
        Longitude = 2.2
        AltitudeInMeters = 3
    }
}

Update-MgPrintConnector -PrintConnectorId $printConnectorId -BodyParameter $params

```