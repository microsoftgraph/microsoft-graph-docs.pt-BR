---
title: Tipo de recurso userRegistrationFeatureCount
description: Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 0a0ad3758a74e057fa5539d3d913dd1735c88854
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052553"
---
# <a name="userregistrationfeaturecount-resource-type"></a>Tipo de recurso userRegistrationFeatureCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|recurso|authenticationMethodFeature|Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha. Os valores possíveis são: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.|
|userCount|Int64|Número de usuários.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
