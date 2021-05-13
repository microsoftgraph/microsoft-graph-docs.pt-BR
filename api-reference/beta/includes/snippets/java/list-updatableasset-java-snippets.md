---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6ebfae16a5994d79ab2f849cccbd6e0452d94e9
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52476727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetCollectionPage exclusions = graphClient.admin().windows().updates().deployments("{deploymentId}").audience().exclusions()
    .buildRequest()
    .get();

```