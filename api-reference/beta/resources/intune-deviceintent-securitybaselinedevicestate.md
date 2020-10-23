---
title: tipo de recurso securityBaselineDeviceState
description: O resumo do estado de conformidade da linha de base de segurança da linha de base de segurança para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33d3b6614957426c48d2f8b9ee9b4ac8b5941ed1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696080"
---
# <a name="securitybaselinedevicestate-resource-type"></a>tipo de recurso securityBaselineDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo do estado de conformidade da linha de base de segurança da linha de base de segurança para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineDeviceStates](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|coleção [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Listar Propriedades e relações dos objetos [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|
|[Obter securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Leia as propriedades e as relações do objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|
|[Criar securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Criar um novo objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|
|[Excluir securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|Nenhum|Exclui [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).|
|[Atualizar securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Atualiza as propriedades de um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade|
|managedDeviceId|String|ID de dispositivo do Intune|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo|
|userPrincipalName|String|Nome UPN|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Estado de conformidade da linha de base de segurança. Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|lastReportedDateTime|DateTimeOffset|Data e hora da última modificação do relatório de política|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





