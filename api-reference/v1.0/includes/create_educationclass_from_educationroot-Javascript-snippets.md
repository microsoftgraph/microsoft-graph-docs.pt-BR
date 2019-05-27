---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8aeea6b1b22d77d4a36c0a257a1a17782a759aee
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: "Health Level 1",
  classCode: "Health 501",
  displayName: "Health 1",
  externalId: "11019",
  externalName: "Health Level 1",
  externalSource: "sis",
  mailNickname: "fineartschool.net"
};

let res = await client.api('/education/classes')
    .post({educationClass : educationClass});

```