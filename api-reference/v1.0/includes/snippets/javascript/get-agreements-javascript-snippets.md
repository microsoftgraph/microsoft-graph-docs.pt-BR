---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46b6f232da763c746924fd9c5e8d337c88a9287a76b52171fa1dde3023509f7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreements = await client.api('/identityGovernance/termsOfUse/agreements')
    .get();

```