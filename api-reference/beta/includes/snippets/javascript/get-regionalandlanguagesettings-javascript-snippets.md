---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0005ffb68b3e7095b56045b00dadfb0076d5623be8c16c757584235929d14cdb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let regionalAndLanguageSettings = await client.api('/me/settings/regionalAndLanguageSettings')
    .version('beta')
    .get();

```