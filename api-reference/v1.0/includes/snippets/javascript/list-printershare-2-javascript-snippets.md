---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65b9c3ef509c41531b9ba6b0898e297e20bfeb3c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shares = await client.api('/print/printers/{printerId}/shares')
    .get();

```