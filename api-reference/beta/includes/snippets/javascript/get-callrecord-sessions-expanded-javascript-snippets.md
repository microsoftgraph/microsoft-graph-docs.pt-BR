---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06da81223c091abe498b8641546313808d4765eb978628c536d0bc50c19fb041
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .version('beta')
    .expand('segments')
    .get();

```