---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81e1c4c9a35be7ddf7641ac719b56819af1762f5f1818f283642f017c7936a4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setVerifiedPublisher = {
    verifiedPublisherId: '1234567'
};

await client.api('/applications/{id}/setVerifiedPublisher')
    .post(setVerifiedPublisher);

```