---
title: tipo de enum clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser fechado. '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034477"
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
