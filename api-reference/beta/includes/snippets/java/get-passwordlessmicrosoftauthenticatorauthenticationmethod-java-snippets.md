---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6754c4f5eda5fe0ad958a890a60c0afa0dde7188
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945805"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordlessMicrosoftAuthenticatorAuthenticationMethod passwordlessMicrosoftAuthenticatorAuthenticationMethod = graphClient.me().authentication().passwordlessMicrosoftAuthenticatorMethods("R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1")
    .buildRequest()
    .get();

```