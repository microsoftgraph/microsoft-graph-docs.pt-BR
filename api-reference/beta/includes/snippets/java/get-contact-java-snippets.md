---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b88dc0b277306a14511d04fc4652709f7d9724f83f007fba19282593af7f6237
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273559"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = graphClient.me().contacts("AAMkAGI2THk0AAA=")
    .buildRequest()
    .get();

```