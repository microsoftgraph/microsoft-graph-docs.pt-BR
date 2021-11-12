---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e13184e606d6bfd76bcbde0ed7c6bfe01b490d7a3261a233374e7d757d2706a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerCapabilities = await client.api('/print/printers/{id}/getCapabilities')
    .version('beta')
    .get();

```