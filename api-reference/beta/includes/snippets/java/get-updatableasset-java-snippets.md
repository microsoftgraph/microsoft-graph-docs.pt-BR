---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 842d45cb93daa0f05f40602c199966a23f0d4939
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAsset updatableAsset = graphClient.admin().windows().updates().updatableAssets("{updatableAssetId}")
    .buildRequest()
    .get();

```