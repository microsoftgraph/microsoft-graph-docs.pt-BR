---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62337497fcfcd66b34f5a427800b013ba5fedb07c85115f8ab0055028eae302e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let definitions = await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```