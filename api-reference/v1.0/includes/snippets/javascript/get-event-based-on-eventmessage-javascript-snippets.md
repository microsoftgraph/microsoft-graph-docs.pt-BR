---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dec80519a2f59724ad233d116be30a7b8ae489d34062c107d6f60fb651404421
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADYAAAImV_jAAA=')
    .expand('eventMessage/event')
    .get();

```