---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f6e72a38e2d9257831cab45eadb0aafce5f9f8a894b79ec351f3b970f32984a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printers = await client.api('/print/printers')
    .version('beta')
    .get();

```