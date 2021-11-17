---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66b402d5c402cd57d46e0643617c04f6f07d8bb9caf072717efd9abc8069e509
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PhoneAuthenticationMethod phoneAuthenticationMethod = new PhoneAuthenticationMethod();
phoneAuthenticationMethod.phoneNumber = "+1 2065555555";
phoneAuthenticationMethod.phoneType = AuthenticationPhoneType.MOBILE;

graphClient.me().authentication().phoneMethods()
    .buildRequest()
    .post(phoneAuthenticationMethod);

```