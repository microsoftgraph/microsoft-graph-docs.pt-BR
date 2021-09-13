---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbe7a7639e1c1ff20e6e5840a259d2700ab4433596370c8751df70edec1b7fe0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897834"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.me().drive()
    .buildRequest()
    .get();

```