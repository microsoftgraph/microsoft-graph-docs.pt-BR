---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 446d6f1f94d40b6b79d6b2651d47ba194da27dca1fd76ba9fe490f45e93926fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .delete();

```