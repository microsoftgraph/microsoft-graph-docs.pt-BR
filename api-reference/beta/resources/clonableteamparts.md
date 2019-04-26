---
title: tipo de enumeração clonableTeamParts
description: 'Descreve que parte de uma equipe deve ser clonada. '
localization_priority: Normal
ms.openlocfilehash: 898b43e054d4b0f010766aef72977d693993afdf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341384"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enumeração clonableTeamParts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve que parte de uma [equipe](../resources/team.md) deve ser clonada. 

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1 |Copie a lista de aplicativos instalados.|
|guias|2 |Copia as guias nos canais.|
|settings|4 |Copia todas as configurações da equipe, juntamente com as configurações de grupo de chaves.|
|channels|8 |Copia a estrutura do canal (mas não as mensagens no canal).|
|membros|16 |Copia os membros e os proprietários da equipe.|
