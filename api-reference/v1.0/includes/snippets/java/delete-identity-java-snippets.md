---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2e97f946174c0492e6a3df6aa82857283efccfd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046133"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").groups("31bea3d537902000").members("14m1b9c38qe647f6a")
    .buildRequest()
    .delete();

```