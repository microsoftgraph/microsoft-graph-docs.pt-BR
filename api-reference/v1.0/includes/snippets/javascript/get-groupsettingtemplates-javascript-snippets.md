---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0e10ad0e1fc50cc1fef24e335ac325763da43d5bb0437d950b42a3089d2a33b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSettingTemplates = await client.api('/groupSettingTemplates')
    .get();

```