---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2f60e77184b69bcf9ab731237feeb53e6fd7922
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091024"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InsightsSettings insightsSettings = graphClient.organization("{organizationId}").settings().itemInsights()
    .buildRequest()
    .get();

```