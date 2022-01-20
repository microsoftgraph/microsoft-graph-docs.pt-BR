---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed859427f2df1100af7fa1847fa85680e21da98d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099608"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListItem -SiteId $siteId -ListId $listId -ListItemId $listItemId -ExpandProperty "fields" 

```