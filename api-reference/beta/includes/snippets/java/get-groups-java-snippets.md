---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4860104dfd5cada609ef1798656b0cc0ec13445b2417f29bdcc7f1584fd90414
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100065"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .get();

```