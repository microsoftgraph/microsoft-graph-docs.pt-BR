---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16d3d84aee26c47e4c24998629a5c821e51dc226f5c4da0573b05fe400fddad2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897828"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.drives("{drive-id}")
    .buildRequest()
    .get();

```