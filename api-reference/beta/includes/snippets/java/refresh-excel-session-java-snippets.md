---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6d430966797a62a4f094aa8f421ea8214178a49314890f84107a416bef05f00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("workbook-session-id", "{session-id}"));

graphClient.me().drive().items("{id}").workbook()
    .refreshSession()
    .buildRequest( requestOptions )
    .post();

```