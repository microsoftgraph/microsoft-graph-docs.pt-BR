---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01f21bd05227238d95dc7c441de273b1dac002cb6d34355b4eac5fdd2ffdf053
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/homeRealmDiscoveryPolicies/{id}/appliesTo')
    .get();

```