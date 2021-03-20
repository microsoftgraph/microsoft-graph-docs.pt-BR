---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5462c4af00ca8312775a4667dd1316cbbece52ff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroupCollectionPage sectionGroups = graphClient.me().onenote().sectionGroups()
    .buildRequest()
    .get();

```