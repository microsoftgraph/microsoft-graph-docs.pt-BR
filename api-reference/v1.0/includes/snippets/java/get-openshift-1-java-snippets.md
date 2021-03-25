---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe87915233b30792f340aa9d41ad09fce7138169
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208563"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShift openShift = graphClient.teams("{id}").schedule().openShifts("OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8")
    .buildRequest()
    .get();

```