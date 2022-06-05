---
title: Tipo de enumeração clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser clonada. '
ms.localizationpriority: medium
author: nkramer
ms.prod: teamwork
doc_type: enumPageType
ms.openlocfilehash: cf317d3487cbd4a29bb860abda4510c2223aec24
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899439"
---
# <a name="clonableteamparts-enum-type"></a>Tipo de enumeração clonableTeamParts

Namespace: microsoft.graph



Descreve qual parte de uma [equipe](../resources/team.md) deve ser clonada.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1|Copie a lista de aplicativos instalados.|
|guias|2|copia as guias dentro dos canais.|
|settings|4|Copia todas as configurações dentro da equipe, juntamente com as configurações do grupo de chaves.|
|channels|8 |copia a estrutura do canal (mas não as mensagens no canal).|
|members|16|copia os membros e proprietários da equipe.|

