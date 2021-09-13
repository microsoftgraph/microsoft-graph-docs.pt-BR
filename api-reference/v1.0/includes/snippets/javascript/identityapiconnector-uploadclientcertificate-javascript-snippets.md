---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48010482583f4cf29bd91b54336fbf0a4aa703a9b60749b34e2ad5e2e155ad4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    pkcs12Value: 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA',
    password: '<password>'
};

await client.api('/identity/apiconnectors/{id}/uploadClientCertificate')
    .post(identityApiConnector);

```