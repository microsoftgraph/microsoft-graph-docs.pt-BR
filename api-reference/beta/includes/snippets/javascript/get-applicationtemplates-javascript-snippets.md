---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f107296ba8c1af4d07bb82d2c92bf6a7a1b7ee18d7d5eac07621474595341cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationTemplates = await client.api('/applicationTemplates')
    .version('beta')
    .get();

```