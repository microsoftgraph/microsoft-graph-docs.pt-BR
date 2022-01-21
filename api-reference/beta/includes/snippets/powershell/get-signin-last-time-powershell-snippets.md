---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3450a3d7b27d4e657106beadf5dd248933c1cf5c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126638"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Property "displayName,userPrincipalName,signInActivity" 

```