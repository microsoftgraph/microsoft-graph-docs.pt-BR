---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91a1dcacb283a39cb43df888407067dfa107fcccae920eb623ff76452bc5a71d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214965"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
Pkcs12Certificate authenticationConfiguration = new Pkcs12Certificate();
authenticationConfiguration.pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";
authenticationConfiguration.password = "secret";
identityApiConnector.authenticationConfiguration = authenticationConfiguration;

graphClient.identity().apiConnectors("be1f769b-9b13-437e-b540-79a905c4932c")
    .buildRequest()
    .patch(identityApiConnector);

```