---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5390abd8234314d73d187a5624a6f429d20ccae6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37998267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/languages/{id}')
    .version('beta')
    .delete();

```