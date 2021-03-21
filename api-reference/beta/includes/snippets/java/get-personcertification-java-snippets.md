---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05548288a97fe0b8f66ca2c85658107520868141
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973863"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertification personCertification = graphClient.me().profile().certifications("{id}")
    .buildRequest()
    .get();

```