---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 242170fbf0be516677ddbeeb48b5090e58c27dd439753e441e7d84de61baf4c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .get();

```