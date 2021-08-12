---
title: Tipo de número clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser clonada. '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 371f026b671f750ef67ec796d154fa3e399ac8967664466bdcb2bc498a11124c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252057"
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
|members|16 |copia os membros e proprietários da equipe.|

