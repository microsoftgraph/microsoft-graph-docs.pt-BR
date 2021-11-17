---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3e818391b11bfcdaa31fe644dcfbb25bcd4f64ca14bbd6c46ff4925f4753a17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898227"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .sendReminder()
    .buildRequest()
    .post();

```