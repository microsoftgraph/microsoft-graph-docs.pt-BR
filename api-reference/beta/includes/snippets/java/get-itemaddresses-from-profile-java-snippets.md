---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c885288c5ae0650655f32f3530f704d0612eb1c7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975914"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddressCollectionPage addresses = graphClient.me().profile().addresses()
    .buildRequest()
    .get();

```