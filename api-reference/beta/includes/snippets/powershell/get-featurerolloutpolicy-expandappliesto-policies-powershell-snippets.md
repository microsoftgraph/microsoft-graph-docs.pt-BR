---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd21700978b1e3dc699a073f614cf827331ec9eb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118862"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyFeatureRolloutPolicy -FeatureRolloutPolicyId $featureRolloutPolicyId -ExpandProperty "appliesTo" 

```