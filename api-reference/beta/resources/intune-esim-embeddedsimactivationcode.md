---
title: Tipo de recurso embeddedSIMActivationCode
description: O código de ativação do SIM incorporado conforme fornecido pela operadora móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68c900ce67f5eff6e7f9f5d9f3078f92fe60686d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787838"
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



