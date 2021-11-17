---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5334242983ab0692245a76e65a68330908036cd4700d88954e03cff93363887b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}/restoreFactoryDefaults')
    .version('beta')
    .post();

```