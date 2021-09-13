---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72e8e0095bfccc7e584afbaf14bc6d6bb7b658a0fba2aa20ab2e8377708cf383
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeBorder = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .get();

```