---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de850ae21d555c52fe62a7f92a5e23deb1764c957c45c0c5944610802935288f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157825"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest()
    .get();

```