---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 994ddcb54186d937f17b0df9235405514a8a2084f32194a5f2c58256479fd094
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214606"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LanguageProficiencyCollectionPage languages = graphClient.me().profile().languages()
    .buildRequest()
    .get();

```