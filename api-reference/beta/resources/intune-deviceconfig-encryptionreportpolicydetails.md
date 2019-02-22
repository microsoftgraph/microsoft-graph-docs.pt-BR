---
title: tipo de recurso encryptionReportPolicyDetails
description: Detalhes da política para o relatório de criptografia
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177914"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>tipo de recurso encryptionReportPolicyDetails

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Detalhes da política para o relatório de criptografia

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|PolicyId|String|ID de política para o relatório de criptografia|
|policyName|String|Nome da política para o relatório de criptografia|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




