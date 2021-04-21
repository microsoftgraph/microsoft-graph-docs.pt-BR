---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a57379975fe1e1c7c4a2dc394531568a71b13a6b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppIcon teamsAppIcon = graphClient.appCatalogs().teamsApps("95de633a-083e-42f5-b444-a4295d8e9314").appDefinitions("OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk").outlineIcon()
    .buildRequest()
    .get();

```