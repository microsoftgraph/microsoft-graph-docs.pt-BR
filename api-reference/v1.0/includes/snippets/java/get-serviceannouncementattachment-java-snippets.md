---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 903c1e13c6e60beb927fc34bad919a6ac3ec85cc
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225694"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/admin/serviceAnnouncement/messages/MC54091/attachments/30356a46-ffad-47e1-acf6-40a99b1538c1/content", InputStream.class)
    .buildRequest()
    .get();

```