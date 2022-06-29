---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80769ef07fd91a77afba91ca29202bb8caa4a1be
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438183"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgApplicationTokenIssuancePolicyByRef -ApplicationId $applicationId -TokenIssuancePolicyId $tokenIssuancePolicyId

```