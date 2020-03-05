---
title: tipo de enumeração clonableTeamParts
description: 'Descreve que parte de uma equipe deve ser clonada. '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 287e63d9972043508c62b29ccf9b72d19accc337
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507653"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enumeração clonableTeamParts

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve que parte de uma [equipe](../resources/team.md) deve ser clonada. 

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1 |Copie a lista de aplicativos instalados.|
|guias|2 |Copia as guias nos canais.|
|configurações|4 |Copia todas as configurações da equipe, juntamente com as configurações de grupo de chaves.|
|channels|8 |Copia a estrutura do canal (mas não as mensagens no canal).|
|membros|16 |Copia os membros e os proprietários da equipe.|
