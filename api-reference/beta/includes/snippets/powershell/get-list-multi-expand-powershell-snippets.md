---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6714ae650ef5d417dbd6c65f445dd39fe706180b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129699"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteList -SiteId $siteId -ListId $listId -Property "name,lastModifiedDateTime" -ExpandProperty "columns(select=name,description),items)" 

```