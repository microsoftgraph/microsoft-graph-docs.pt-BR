---
title: tipo de enum clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser fechado. '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860554"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enum clonableTeamParts

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Descreve qual parte de uma [equipe](../resources/team.md) deve ser fechado. 

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Aplicativos|1|Copie a lista de aplicativos instalados.|
|guias|2|copia as guias no canais.|
|configurações|4|Copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.|
|canais|8|Copia a estrutura de canal (mas não as mensagens no canal).|
|membros|16|copia os membros e proprietários da equipe.|
