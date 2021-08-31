---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad6f863810c4d3ce0407cff35c3cfef154645f9e281590c1f6277b07be14674b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserInsightsSettings userInsightsSettings = graphClient.me().settings().itemInsights()
    .buildRequest()
    .get();

```