---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69e7f7a742847750cfd519c93a07dfcd84b939aa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953247"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=").taskFolders()
    .buildRequest()
    .get();

```