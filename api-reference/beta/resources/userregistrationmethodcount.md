---
title: Tipo de recurso userRegistrationMethodCount
description: Número de usuários registrados para um método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 8e4c19c48771ccd0bd1dd1f1a4b049334266834a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132928"
---
# <a name="userregistrationmethodcount-resource-type"></a>Tipo de recurso userRegistrationMethodCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Número de usuários registrados para um método de autenticação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationMethod|String|Nome do método de autenticação.|
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
