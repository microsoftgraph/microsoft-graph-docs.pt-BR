---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04adda6beb76eb2dc7369a7e4d0dbebe11691da73664ad6090dd7483dfa416c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273403"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PhoneAuthenticationMethod phoneAuthenticationMethod = new PhoneAuthenticationMethod();
phoneAuthenticationMethod.phoneNumber = "+1 2065555554";
phoneAuthenticationMethod.phoneType = AuthenticationPhoneType.MOBILE;

graphClient.me().authentication().phoneMethods("3179e48a-750b-4051-897c-87b9720928f7")
    .buildRequest()
    .put(phoneAuthenticationMethod);

```