---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f70e0f1c5c694073d1b0874b576828ce3606cb8fe944c951667673fe50fbabcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100185"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PhoneAuthenticationMethodCollectionPage phoneMethods = graphClient.me().authentication().phoneMethods()
    .buildRequest()
    .get();

```