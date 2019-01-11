---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76c13c26812fd8ab7c8e1224b55e616502b514ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839267"
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



