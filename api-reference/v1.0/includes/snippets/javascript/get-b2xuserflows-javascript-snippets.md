---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 208da044e06f9f296aaac27386eced271cf4c6ec
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xIdentityUserFlow = await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp')
    .get();

```