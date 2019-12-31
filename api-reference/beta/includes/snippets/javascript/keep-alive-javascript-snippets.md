---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66922b440dbccb729e13ecc69fe82b8a3f9bf7ec
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive')
    .version('beta')
    .post();

```