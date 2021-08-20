---
title: Tipo de recurso embeddedSIMActivationCode
description: O código de ativação do SIM incorporado conforme fornecido pela operadora móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07acfbad5baf0cb68118472ea32d667c7f2868dac490665e61726fd5a6e4bf75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242563"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Tipo de recurso embeddedSIMActivationCode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O código de ativação do SIM incorporado conforme fornecido pela operadora móvel.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|integratedCircuitCardIdentifier|Cadeia de caracteres|O Identificador de Placa de Circuito Integrado (ICCID) para este código de ativação de SIM incorporado conforme fornecido pela operadora móvel.
A entrada deve corresponder à seguinte expressão regular: '^ \[ 0-9 \] {19} \[ 0-9 \] ?$'.|
|matchingIdentifier|Cadeia de caracteres|O MatchingIdentifier (MatchingID) conforme especificado na Seção Especificação Técnica da Associação GSMA SGP.22 RSP 4.1.
A entrada deve corresponder à seguinte expressão regular: '^ \[ a-zA-Z0-9 \- \] *$'.|
|smdpPlusServerAddress|Cadeia de caracteres|O nome de domínio totalmente qualificado do servidor SM-DP+ conforme especificado na Especificação Técnica do RSP da Associação GSM SPG .22.
A entrada deve corresponder à seguinte expressão regular: '^( \[ a-zA-Z0-9 \] +(- \[ a-zA-Z0-9 \] +)* \. )+ \[ a-zA-Z \] {2,} $'.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```




