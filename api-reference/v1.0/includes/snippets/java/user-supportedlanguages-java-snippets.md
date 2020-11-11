---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f08147e08f0afdf596b72f9025d16ff0580608a7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983738"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookUserSupportedLanguagesCollectionPage supportedLanguages = graphClient.me().outlook()
    .supportedLanguages()
    .buildRequest()
    .get();

```