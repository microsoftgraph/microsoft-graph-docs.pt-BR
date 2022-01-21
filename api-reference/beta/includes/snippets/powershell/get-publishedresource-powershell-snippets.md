---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5a9d1bae48bca8ac3aefd9cf32669fdcb0a3cce
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105601"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfilePublishedResource -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -PublishedResourceId $publishedResourceId -ExpandProperty "agentGroups" 

```