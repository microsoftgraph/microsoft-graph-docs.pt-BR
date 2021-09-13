---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f64feb1b0b6c0de5505351e5d6b42fd69a57ec6c39d90a3f322d22cebd27f86c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters')
    .post();

```