---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c931ceea238e45990211e84b9725815b8f409117
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953612"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/me/schools')
    .get();

```