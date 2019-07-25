---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7515d75c4b081f106a20eb6291e16a6cb6bb8b53
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856277"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String password = "password-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").protection()
    .unprotect()
    .buildRequest()
    .post();

```