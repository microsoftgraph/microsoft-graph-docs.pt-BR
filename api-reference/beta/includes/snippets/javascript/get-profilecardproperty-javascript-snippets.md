---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51e1a01ce7a0cc8e094d512c6cbbf0a4954033bd6d6ee8a39168edb982d67b8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profileCardProperty = await client.api('/organization/{organizationId}/settings/profileCardProperties/{id}')
    .version('beta')
    .get();

```