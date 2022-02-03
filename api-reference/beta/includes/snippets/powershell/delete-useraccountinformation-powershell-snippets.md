---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8398cfb5c166a0ed8f1b533dd3d1d154f9bd4d91
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351616"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileAccount -UserId $userId -UserAccountInformationId $userAccountInformationId

```