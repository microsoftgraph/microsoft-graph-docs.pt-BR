---
title: tipo de enumeração clonableTeamParts
description: 'Descreve que parte de uma equipe deve ser clonada. '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 5d9121d7cbaa10260b1a7a7ce180ed7c9f37a565
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086806"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enumeração clonableTeamParts

Namespace: microsoft.graph



Descreve que parte de uma [equipe](../resources/team.md) deve ser clonada.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1 |Copie a lista de aplicativos instalados.|
|guias|2 |Copia as guias nos canais.|
|configurações|4 |Copia todas as configurações da equipe, juntamente com as configurações de grupo de chaves.|
|channels|8 |Copia a estrutura do canal (mas não as mensagens no canal).|
|membros|16 |Copia os membros e os proprietários da equipe.|

