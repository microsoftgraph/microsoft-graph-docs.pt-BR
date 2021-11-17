---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a8dc19761ef4a9ee1ea65df8371468a7f4b05e7ac6b89b73b994e746380b405
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=')
    .version('beta')
    .delete();

```