---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d7ca2914d5b455e834479dbb3ef9d3b52a02148
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112267"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    Name = "name-value"
    "Printer@odata.bind" = "https://graph.microsoft.com/beta/print/printers/{id}"
}

New-MgPrintShare -BodyParameter $params

```