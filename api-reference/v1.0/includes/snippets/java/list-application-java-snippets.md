---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0304ed0a2a082e8f3cb9176c1d68c48aa5994c3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IApplicationCollectionPage applications = graphClient.applications()
    .buildRequest()
    .get();

```