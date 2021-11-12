---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2aac851f92e782f88fd591cb46cf1075905a0c72429d752170732530f04bf27f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  color: 'color-value',
  style: 'style-value',
  sideIndex: 'sideIndex-value',
  weight: 'weight-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .version('beta')
    .update(workbookRangeBorder);

```