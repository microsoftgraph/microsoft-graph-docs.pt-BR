---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a10c7b36e074dbf75e4e7b9bd61d3eea2d70d915479297b0a76c14899c53cf7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#Microsoft.OutlookServices.ItemAttachment',
  name: 'name-value',
  item: {
    '@odata.type': 'microsoft.graph.message'
  }
};

await client.api('/me/events/{id}/attachments')
    .version('beta')
    .post(attachment);

```