---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc0bd4c7183ca9440f3702fff5b1eab143703a5c26b463cb4c4b12251bccc819
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100968"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```