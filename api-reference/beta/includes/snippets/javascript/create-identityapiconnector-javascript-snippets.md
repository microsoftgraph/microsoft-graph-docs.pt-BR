---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 854765fd5eaef5d9e9aa9cbc1ce7f972cced487cf798b156538ef5b43ddc6de3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    displayName: 'Test API',
    targetUrl: 'https://someotherapi.com/api',
    authenticationConfiguration: {
        '@odata.type':'#microsoft.graph.pkcs12Certificate',
        pkcs12Value: 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA',
        password: '<password>'
    }
};

await client.api('/identity/apiConnectors')
    .version('beta')
    .post(identityApiConnector);

```