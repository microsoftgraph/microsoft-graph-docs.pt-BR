---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 266dc55dc8d7a6dd8bbcd84c090c6742f5765cb0
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcGalleryImageCollectionPage galleryImages = graphClient.deviceManagement().virtualEndpoint().galleryImages()
    .buildRequest()
    .get();

```