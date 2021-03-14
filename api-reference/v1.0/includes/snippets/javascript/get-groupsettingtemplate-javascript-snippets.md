---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbe54862ab35084c58ab32023523af03d48ad1fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSettingTemplate = await client.api('/groupSettingTemplates/{id}')
    .get();

```