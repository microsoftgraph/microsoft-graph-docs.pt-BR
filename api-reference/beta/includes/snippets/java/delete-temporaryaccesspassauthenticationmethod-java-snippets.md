---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95a30c168c0dd7b9471e582357fcb0b8eb7f701a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("071cc716-8147-4397-a5ba-b2105951cc0b").authentication().temporaryAccessPassMethods("05267842-25b2-4b21-8abd-8e4982796f7f")
    .buildRequest()
    .delete();

```