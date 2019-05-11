---
title: tipo de recurso securityBaselineDeviceState
description: O resumo do estado de conformidade da linha de base de segurança da linha de base de segurança para um dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff87b5c39d00957ddd4128bc3351879dcd5b652f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943288"
---
# <a name="securitybaselinedevicestate-resource-type"></a>tipo de recurso securityBaselineDeviceState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|managedDeviceId|Cadeia de caracteres|ID de dispositivo do Intune|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo|
|userPrincipalName|Cadeia de caracteres|Nome UPN|
|estado|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Estado de conformidade da linha de base de segurança. Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
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




