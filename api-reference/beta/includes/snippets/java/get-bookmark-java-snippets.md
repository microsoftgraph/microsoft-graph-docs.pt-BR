---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aadb636be81b4cde69e3d14f058d9a635b259bb6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338053"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Bookmark bookmark = graphClient.search().bookmarks("{bookmarksId}")
    .buildRequest()
    .get();

```