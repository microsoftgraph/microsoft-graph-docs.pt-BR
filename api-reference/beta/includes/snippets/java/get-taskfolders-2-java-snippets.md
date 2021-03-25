---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12f9583af09dcbbd40301b84c33ac83dab1f390d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskFolders()
    .buildRequest()
    .get();

```