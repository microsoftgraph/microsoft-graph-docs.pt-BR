---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19341b52fe1a33813622f04d7c1949ae96f20166
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{updatableAssetId}")
    .buildRequest()
    .delete();

```