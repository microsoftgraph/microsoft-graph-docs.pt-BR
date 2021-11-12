---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d21dc9924fbefacec076c3996bd0389e73ffe8dd38ee184662a6877627572d2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userSource = {
  email: 'adelev@contoso.com',
  includedSources: 'mailbox'
};

await client.api('/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources')
    .version('beta')
    .post(userSource);

```