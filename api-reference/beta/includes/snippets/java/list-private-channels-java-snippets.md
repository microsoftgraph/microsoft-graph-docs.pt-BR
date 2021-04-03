---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7d6ac2dab8d65b91853e8ded95da8fbbaaeb4f7
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("64c323f2-226a-4e64-8ba4-3e6e3f7b9330").channels()
    .buildRequest()
    .filter("membershipType eq 'private'")
    .get();

```