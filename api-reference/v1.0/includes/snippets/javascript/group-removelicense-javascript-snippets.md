---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de9330e10ec2bb1029075edef90e662168114551
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953667"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  addLicenses: [],
  removeLicenses: ["skuId-value-1", "skuId-value-2"]
};

let res = await client.api('/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense')
    .post(group);

```