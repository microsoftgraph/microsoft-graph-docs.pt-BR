---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3440340b6d3fbfa403609c3271bdd96352ea9003bdfb3adfa320bfb1a13c5f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214575"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .buildRequest()
    .delete();

```