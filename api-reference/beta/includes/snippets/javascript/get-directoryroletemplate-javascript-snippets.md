---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e357e698741bfae702258bb68492c2d8175a848444cd0a646d34c8ab48dad8f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplate = await client.api('/directoryRoleTemplates/{id}')
    .version('beta')
    .get();

```