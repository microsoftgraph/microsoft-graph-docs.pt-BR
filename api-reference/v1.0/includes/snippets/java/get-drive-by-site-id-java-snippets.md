---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2207e37c2b5d531f4a13f7ca6ae2fa8f8a9ea8e4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887867"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.sites("{siteId}").drive()
    .buildRequest()
    .get();

```