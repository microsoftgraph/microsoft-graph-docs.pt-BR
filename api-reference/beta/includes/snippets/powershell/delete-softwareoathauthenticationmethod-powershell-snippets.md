---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00c1d7c972336b8f2bf7156ee380eb44c37ef91d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130805"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationSoftwareOathMethod -UserId $userId -SoftwareOathAuthenticationMethodId $softwareOathAuthenticationMethodId

```