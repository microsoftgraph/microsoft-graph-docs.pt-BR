---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c747a9321f1995bf11823a43ea78896ad6e5882c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveRecentCollectionPage recent = graphClient.me().drive()
    .recent()
    .buildRequest()
    .get();

```