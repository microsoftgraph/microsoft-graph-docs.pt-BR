---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3ff8d4046fc3a32a0a4450ee822acf8681ebc31
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951591"
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