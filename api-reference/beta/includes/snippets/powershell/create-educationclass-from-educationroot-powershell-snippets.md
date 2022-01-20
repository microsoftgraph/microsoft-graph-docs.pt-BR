---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9ffb58313c6380ff76dd7d43b672bcbbc5f99d7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090198"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Description = "Health Level 1"
    ClassCode = "Health 501"
    DisplayName = "Health 1"
    ExternalId = "11019"
    ExternalName = "Health Level 1"
    ExternalSource = "sis"
    MailNickname = "fineartschool.net"
}

New-MgEducationClass -BodyParameter $params

```