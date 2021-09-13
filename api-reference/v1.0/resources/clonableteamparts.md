---
title: Tipo de número clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser clonada. '
ms.localizationpriority: medium
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 29ed2da8079d00576d19e94d792da0b1af423781
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109280"
---
# <a name="clonableteamparts-enum-type"></a>Tipo de número clonableTeamParts

Namespace: microsoft.graph



Descreve qual parte de uma [equipe](../resources/team.md) deve ser clonada.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|apps|1|Copie a lista de aplicativos instalados.|
|guias|2|copia as guias dentro dos canais.|
|settings|4 |Copia todas as configurações dentro da equipe, juntamente com as principais configurações de grupo.|
|channels|8 |copia a estrutura do canal (mas não as mensagens no canal).|
|membros|16 |copia os membros e proprietários da equipe.|

