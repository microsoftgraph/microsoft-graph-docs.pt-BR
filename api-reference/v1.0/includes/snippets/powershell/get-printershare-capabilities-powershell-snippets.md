---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9092b08d0ac21cebbc307cc2851e035dce658db9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091951"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Get-MgPrintShare -PrinterShareId $printerShareId -Property "id,displayName,capabilities" 

```