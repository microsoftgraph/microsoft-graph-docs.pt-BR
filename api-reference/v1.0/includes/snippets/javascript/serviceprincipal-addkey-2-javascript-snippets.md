---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2aaff6ecd97d343b9bc22c183cfe47f541735652be4de4b2a2488c7cb752357
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const keyCredential = {
    keyCredential: {
        type: 'X509CertAndPassword',
        usage: 'Sign',
        key: 'MIIDYDCCAki...'
    },
    passwordCredential: {
        secretText: 'MKTr0w1...'
    },
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/servicePrincipals/{id}/addKey')
    .post(keyCredential);

```