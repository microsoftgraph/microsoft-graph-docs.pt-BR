---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7a7b740cb8061bfca305701840f9c9335f1e79f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .header('ConsistencyLevel','eventual')
    .filter('hasMembersWithLicenseErrors+eq+true,')
    .select('id,displayName')
    .get();

```