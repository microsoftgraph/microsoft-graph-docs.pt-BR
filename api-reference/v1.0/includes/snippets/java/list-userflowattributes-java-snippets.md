---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6562899abf0064689dacedbc206ba849319b9b17
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeCollectionPage userFlowAttributes = graphClient.identity().userFlowAttributes()
    .buildRequest()
    .get();

```