---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8115501ec691578e30690e83949355c25cdec25
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239320"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}")
    .buildRequest()
    .delete();

```