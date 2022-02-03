---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba06eed5a76a63ccf7a96fa9c455eb0d620bec6a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344577"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    ContentTypeId = "String"
}

Add-MgSiteListContentTypeCopyFromContentTypeHub -SiteId $siteId -ListId $listId -BodyParameter $params

```