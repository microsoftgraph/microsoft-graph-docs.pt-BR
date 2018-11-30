---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
ms.openlocfilehash: 2733723252f3b8f03cf08fda6d0b09f207ae5550
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007181"
---
# <a name="applisttype-enum-type"></a>tipo de enum appListType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Possíveis valores da lista de aplicativos de conformidade.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|0|Valor padrão, sem intenção.|
|appsInListCompliant|1|A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).|
|appsNotInListCompliant|2|A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).|



