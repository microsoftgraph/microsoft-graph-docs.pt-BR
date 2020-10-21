---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70a28849083f8fd6bcacc9fdfa777859a5fcf5a3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .filter('hasMembersWithLicenseErrors+eq+true,')
    .select('id,displayName')
    .get();

```