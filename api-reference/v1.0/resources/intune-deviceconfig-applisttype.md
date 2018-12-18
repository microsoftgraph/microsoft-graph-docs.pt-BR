---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354716"
---
# <a name="applisttype-enum-type"></a>tipo de enum appListType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Possíveis valores da lista de aplicativos de conformidade.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Valor padrão, sem intenção.|
|appsInListCompliant|1|A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).|
|appsNotInListCompliant|2|A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).|



