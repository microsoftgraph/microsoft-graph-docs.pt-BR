---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1582fa5023c41a38b90a9da5bb884570845b86ea
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126324"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListItemVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -ListItemVersionId $listItemVersionId -ExpandProperty "fields" 

```