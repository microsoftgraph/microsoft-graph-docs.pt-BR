---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb7f153bdc21dac0f43c69af5889523134e33effed498b5c5483225abf9699a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6'
};

await client.api('/servicePrincipals/{id}/removePassword')
    .post(removePassword);

```