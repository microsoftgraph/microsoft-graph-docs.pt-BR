---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc463cd15ddbd15e009805b9517cf4a7a02dad00b6ed30fb81363d97b9efb457
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```