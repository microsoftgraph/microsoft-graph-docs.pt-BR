---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6320cddb5c7820b46346ec849c94f5e6883486a1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("workbook-session-id", "{session-id}"));

graphClient.me().drive().items("{id}").workbook()
    .closeSession(this)
    .buildRequest( requestOptions )
    .post();

```