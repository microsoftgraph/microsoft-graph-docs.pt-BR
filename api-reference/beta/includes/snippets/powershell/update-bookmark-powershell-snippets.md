---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0a8bd1b1c87156c1bdffbf7f383939e9541ed06
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337982"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Description = "Book a fancy vacation in Tuscany or browse museums in Florence."
}

Update-MgSearchBookmark -BookmarkId $bookmarkId -BodyParameter $params

```