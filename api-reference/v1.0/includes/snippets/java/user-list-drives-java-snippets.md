---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf0f48c162f1ab2dc74551aaeaeb18f08881d86c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975967"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.users("{userId}").drives()
    .buildRequest()
    .get();

```