---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1819309e4e4ae0d4b0f7578051dff79bc404c9c1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209486"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EndpointCollectionPage endpoints = graphClient.groups("{id}").endpoints()
    .buildRequest()
    .get();

```