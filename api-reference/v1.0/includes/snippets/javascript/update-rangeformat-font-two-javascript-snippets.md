---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03b30c06b173b21e5e54c2435911521baba6440bba75391b3e5017ff7346fede
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  italic: true,
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font')
    .update(workbookRangeFont);

```