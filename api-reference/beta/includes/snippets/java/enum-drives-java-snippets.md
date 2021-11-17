---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 530512e0baa60947049805a5e43473e4650798cbf1b0ae21105da6e5fc61d3af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157262"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.me().drives()
    .buildRequest()
    .get();

```