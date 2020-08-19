---
title: tipo de enumeração clonableTeamParts
description: 'Descreve que parte de uma equipe deve ser clonada. '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: nkramer
ms.openlocfilehash: e08beeb232e5c9b2c77200f75053e3a822945ca6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810584"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enumeração clonableTeamParts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve que parte de uma [equipe](../resources/team.md) deve ser clonada.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1|Copie a lista de aplicativos instalados.|
|guias|duas|Copia as guias nos canais.|
|configurações|4 |Copia todas as configurações da equipe, juntamente com as configurações de grupo de chaves.|
|channels|8 |Copia a estrutura do canal (mas não as mensagens no canal).|
|members|16 |Copia os membros e os proprietários da equipe.|
