---
title: Tipo de enumeração clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser clonada. '
ms.localizationpriority: medium
doc_type: enumPageType
ms.prod: teamwork
author: nkramer
ms.openlocfilehash: 99a50eb62af486b1d5eb84ae779627bbf8509cc1
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944138"
---
# <a name="clonableteamparts-enum-type"></a>Tipo de enumeração clonableTeamParts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve qual parte de uma [equipe](../resources/team.md) deve ser clonada.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1|Copie a lista de aplicativos instalados.|
|guias|2|copia as guias dentro dos canais.|
|settings|4|Copia todas as configurações dentro da equipe, juntamente com as configurações do grupo de chaves.|
|channels|8 |copia a estrutura do canal (mas não as mensagens no canal).|
|members|16|copia os membros e proprietários da equipe.|


