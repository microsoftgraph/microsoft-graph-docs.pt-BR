---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a58e08d3f9432fa6ed0be36f50abe777775c6881fff51ffcb5f274b62e7be6fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}')
    .delete();

```