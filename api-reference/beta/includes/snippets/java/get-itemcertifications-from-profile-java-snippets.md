---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87a9021c0042ec1c5bf41011b1ab3516a5b9a450
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertificationCollectionPage certifications = graphClient.me().profile().certifications()
    .buildRequest()
    .get();

```