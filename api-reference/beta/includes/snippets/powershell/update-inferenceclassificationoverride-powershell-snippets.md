---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70a25c006d2c311dd45db90812fd14ec4be40371
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350584"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ClassifyAs = "focused"
}

# A UPN can also be used as -UserId.
Update-MgUserInferenceClassificationOverride -UserId $userId -InferenceClassificationOverrideId $inferenceClassificationOverrideId -BodyParameter $params

```