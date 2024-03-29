---
title: Tipo de recurso securityBaselineDeviceState
description: O resumo do estado de conformidade da linha de base de segurança de um dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f960ec9f9a0b56b8a28cda555cf78514cebb0bbb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051248"
---
# <a name="securitybaselinedevicestate-resource-type"></a>Tipo de recurso securityBaselineDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo do estado de conformidade da linha de base de segurança de um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineDeviceStates](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|[coleção securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Listar propriedades e relações dos [objetos securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|
|[Obter securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Leia propriedades e relações do [objeto securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|
|[Criar securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Crie um novo [objeto securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|
|[Excluir securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|Nenhum|Exclui um [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).|
|[Atualizar securityBaselineDeviceState](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Atualize as propriedades de [um objeto securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade|
|managedDeviceId|Cadeia de Caracteres|ID de dispositivo do Intune|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo|
|userPrincipalName|Cadeia de caracteres|Nome UPN|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Estado de conformidade da linha de base de segurança. Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|lastReportedDateTime|DateTimeOffset|Data da última modificação do relatório de política|

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



