---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02895639d3a6681bfc9553864494b87d92b21b8a8ae9cd85db3965d98b96d4f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printSettings = await client.api('/print/settings')
    .version('beta')
    .get();

```