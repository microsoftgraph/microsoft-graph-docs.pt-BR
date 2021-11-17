---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42c3383b8a9dcf2ca0875fc3a9cacbffb817c632cfb8cbe95a01d6540d4321f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest()
    .get();

```