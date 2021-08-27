---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bce54534ed23d4cc22cbb24705f5d7a97ad4a580ca2f6d11a86667f95e2c8033
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/identityProviders/{id}')
    .version('beta')
    .delete();

```