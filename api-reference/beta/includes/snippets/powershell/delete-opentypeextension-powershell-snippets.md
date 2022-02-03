---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d70adfb25247382b3073be97f256f11f9ff7abc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352032"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Remove-MgUserMessageExtension -UserId $userId -MessageId $messageId -ExtensionId $extensionId

```