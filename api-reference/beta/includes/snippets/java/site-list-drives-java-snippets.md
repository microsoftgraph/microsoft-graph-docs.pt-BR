---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cff3929e2590eb440e02f46810dd026776b3fc3d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977559"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.sites("{siteId}").drives()
    .buildRequest()
    .get();

```