---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28aea918c35bb9d90f514e4a8838f219c212405b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830853"
---
# <a name="safesearchfiltertype-enum-type"></a>tipo de enum safeSearchFilterType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|estrito|1|Restrito, mais alto de filtragem em relação a conteúdo para adultos.|
|moderar|2|Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).|



