---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: beaf797b0dc1d9634447151b74ead9ae0e9f66f2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881334"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhAAAW-VPeAAA=")
    .buildRequest()
    .select("internetMessageHeaders")
    .get();

```