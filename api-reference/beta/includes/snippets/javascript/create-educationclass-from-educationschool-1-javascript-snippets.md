---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25e682bef0b833c562ca9587d32ca0d327c5f51f18a44f993d98818a50c9539f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11003/members/14008')
    .version('beta')
    .delete();

```