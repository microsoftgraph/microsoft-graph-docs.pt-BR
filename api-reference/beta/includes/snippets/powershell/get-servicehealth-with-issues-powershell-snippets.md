---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7663571e2fa3ee7639894bf9443ba93d0d69f6c2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397145"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

Get-MgServiceAnnouncementHealthOverview -ServiceHealthId $serviceHealthId -ExpandProperty "issues" 

```