---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3de119678568a72a02c46999f2f9abe9cf72cbb92850b31042e8d7f1c1dd07d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213940"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Accept-Language", "fr"));

InputStream stream = graphClient.customRequest("/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo", InputStream.class)
    .buildRequest( requestOptions )
    .get();

```