---
title: Tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ae128466c0817dedb8e0ae435246a958967bba7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063654"
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
|failureDetails|Cadeia de Caracteres|A descrição detalhada do que deu errado.|
|correção|String|A descrição detalhada de como remediar esse problema.|
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




