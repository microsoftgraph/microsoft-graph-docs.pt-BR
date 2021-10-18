---
title: tipo de recurso continuousAccessEvaluationSessionControl
description: Controle de sessão para controlar as configurações de avaliação de acesso contínuo.
author: lujiangfeng666
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: caa6c09d54d2305af348b848d99e0e43049f5c55
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450787"
---
# <a name="continuousaccessevaluationsessioncontrol-resource-type"></a>tipo de recurso continuousAccessEvaluationSessionControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Controle de sessão para controlar as configurações de avaliação de acesso contínuo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|modo|continuousAccessEvaluationMode| Especifica as configurações de avaliação de acesso contínuo. Os valores possíveis são: `strictEnforcement`, `disabled`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationSessionControl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationSessionControl",
  "mode": "String"
}
```
