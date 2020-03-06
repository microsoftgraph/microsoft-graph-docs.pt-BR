---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1713b4d1149acc9bf169847a444481e6493e5141
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: "Display name"
};

let res = await client.api('/applications')
    .post(application);

```