---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04b6b7d0dae68e9c6a34411424e256078f88255c
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891101"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcGalleryImage cloudPcGalleryImage = graphClient.deviceManagement().virtualEndpoint().galleryImages("{id}")
    .buildRequest()
    .get();

```