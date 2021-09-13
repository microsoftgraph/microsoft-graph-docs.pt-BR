---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c02d04ff64fa5f4e426f2972257f9eb572e56efee16f2c66685ed7c10443ba70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: '#0000FF'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill')
    .update(workbookRangeFill);

```