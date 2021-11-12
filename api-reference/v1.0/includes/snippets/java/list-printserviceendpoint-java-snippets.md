---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 206f82323d758d3bf3be5e9c4df576aedf44b18791dfb64dd5e028beab1886de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216473"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{printServiceId}").endpoints()
    .buildRequest()
    .get();

```