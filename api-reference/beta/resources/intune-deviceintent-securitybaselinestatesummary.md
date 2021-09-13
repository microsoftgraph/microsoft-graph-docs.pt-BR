---
title: Tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 962fc60b94cda4407283f9b6609f03b79d378e27
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069002"
---
# <a name="securitybaselinestatesummary-resource-type"></a>Tipo de recurso securityBaselineStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter securityBaselineStateSummary](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Leia propriedades e relações do [objeto securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|[Atualizar securityBaselineStateSummary](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Atualize as propriedades de [um objeto securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|secureCount|Int32|Número de dispositivos seguros|
|notSecureCount|Int32|Número de dispositivos não seguros|
|unknownCount|Int32|Número de dispositivos desconhecidos|
|errorCount|Int32|Número de dispositivos com erro|
|conflictCount|Int32|Número de dispositivos em conflito|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```



