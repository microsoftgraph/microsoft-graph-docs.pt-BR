---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86f4b0af6521396694567b33992334a1c956f301
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984380"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskGroupCollectionPage taskGroups = graphClient.me().outlook().taskGroups()
    .buildRequest()
    .get();

```