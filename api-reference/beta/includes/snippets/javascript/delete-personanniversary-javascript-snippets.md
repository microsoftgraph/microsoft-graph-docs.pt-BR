---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44c645b3b07b8f82d4d4053dd140cbd6343a6f01e0e24b1a483c18221356586c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .delete();

```