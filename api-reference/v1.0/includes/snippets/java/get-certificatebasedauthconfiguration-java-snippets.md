---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09c35e1de2df8b358c4b296372be645a08be96ef
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979726"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfiguration certificateBasedAuthConfiguration = graphClient.organization("{id}").certificateBasedAuthConfiguration("{id}")
    .buildRequest()
    .get();

```