---
title: tipo de enumeração clonableTeamParts
description: 'Descreve que parte de uma equipe deve ser clonada. '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: nkramer
ms.openlocfilehash: 666dc3cc60490a9a30a5e2bab0b0642c34fb5009
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034074"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enumeração clonableTeamParts

Namespace: microsoft.graph

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


