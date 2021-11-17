---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4794deb96b98e297dc7455ce790cbf2450b3499493dd5367aeaa964fe662ef43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: 'MSGraph Sample',
  isViewingBeforeAcceptanceRequired: true,
  files: [
    {
      fileName: 'TOU.pdf',
      language: 'en',
      isDefault: true,
      fileData: {
        data: 'SGVsbG8gd29ybGQ='
      }
    }
  ]
};

await client.api('/identityGovernance/termsOfUse/agreements')
    .version('beta')
    .post(agreement);

```