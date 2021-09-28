---
title: Tipo de recurso attackSimulationUser
description: Usuário em uma campanha de treinamento e simulação de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 961a8af1bed831b019f41ddf6a7643ac3b26ab07
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979452"
---
# <a name="attacksimulationuser-resource-type"></a>Tipo de recurso attackSimulationUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um usuário em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição do usuário.|
|email|Cadeia de caracteres|Endereço de email do usuário.|
|userId|Cadeia de caracteres|Esse é o **valor da propriedade id** do recurso [do](../resources/user.md) usuário que representa o usuário no locatário do Azure AD.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationUser",
  "userId": "String",
  "displayName": "String",
  "email": "String"
}
```

