---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ceb957689633dcd7f163a6a20ca0f244e2ad4b48c9ac658345f276bd3169af0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/classes/11014/schools')
    .version('beta')
    .get();

```