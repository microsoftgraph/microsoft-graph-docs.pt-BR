---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79d8eaaf485f8bddf2b4595e73abfeda6b4646f0b47459d793985ddb9da0bda5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shares = await client.api('/print/printers/{printerId}/shares')
    .get();

```