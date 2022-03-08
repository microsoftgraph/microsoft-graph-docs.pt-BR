---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c35069d5d85fc85d6a0f016ec923415ceb023113
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338176"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookmarkCollectionPage bookmarks = graphClient.search().bookmarks()
    .buildRequest()
    .get();

```