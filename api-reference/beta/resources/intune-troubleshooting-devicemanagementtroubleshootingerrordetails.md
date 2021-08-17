---
title: Tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c67de7db6a74c327e765e13a6440c7ec6bf3a1ce
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58248162"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>Tipo de recurso deviceManagementTroubleshootingErrorDetails

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Objeto contendo informações detalhadas sobre o erro e sua correção.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|context|String|Ainda não documentado|
|failure|String|Ainda não documentado|
|failureDetails|Cadeia de caracteres|A descrição detalhada do que deu errado.|
|correção|Cadeia de caracteres|A descrição detalhada de como remediar esse problema.|
|recursos|[Coleção deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)|Links para documentação útil sobre essa falha.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




