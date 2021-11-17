---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc354bd75b55d79619121bde0be0cf06104a7440a9e2de70258026637208445b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275579"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAsset updatableAsset = graphClient.admin().windows().updates().updatableAssets("983f03cd-03cd-983f-cd03-3f98cd033f98")
    .buildRequest()
    .get();

```