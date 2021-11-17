---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2f3b911d5e20653a7150caae5eb072bfb668235d7e7e71a94803f47bf795217
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAsset updatableAsset = graphClient.admin().windows().updates().updatableAssets("{updatableAssetId}")
    .buildRequest()
    .get();

```