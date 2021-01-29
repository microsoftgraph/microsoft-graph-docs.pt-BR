---
title: Tipo de recurso userRegistrationMethodCount
description: Número de usuários registrados para um método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: b61cb0448c131fc49df43154522e587644d13dc6
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052559"
---
# <a name="userregistrationmethodcount-resource-type"></a>Tipo de recurso userRegistrationMethodCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Número de usuários registrados para um método de autenticação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationMethod|Cadeia de caracteres|Nome do método de autenticação.|
|userCount|Int64|Número de usuários registrados.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```