---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4ae70ff265f126c5fafb4f8f5bab780fd7319396b738c488899a2f32ead7eea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216329"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomCollectionPage rooms = graphClient.places("bldg2@contoso.com").microsoft.graph.roomlist().rooms()
    .buildRequest()
    .get();

```