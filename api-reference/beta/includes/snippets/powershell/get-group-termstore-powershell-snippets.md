---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e481c140a292e3217dfb8ba767b9a81c59cf439a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440115"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteTermStoreGroup -SiteId $siteId -GroupId $groupId -Property "*,parentSiteId" 

```