---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37bec603aaa2549ff8193829f7a6106be11dd718
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107737"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationCallRecordSession -CallRecordId $callRecordId -ExpandProperty "segments" 

```