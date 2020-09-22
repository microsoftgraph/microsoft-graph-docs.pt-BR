---
title: tipo de recurso deviceManagementIntentUserState
description: Entidade que representa o estado do usuário para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88b27f3f5d651f46d4560059e57ed5322c5154be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061326"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>tipo de recurso deviceManagementIntentUserState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o estado do usuário para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentUserStates](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|coleção [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Listar Propriedades e relações dos objetos [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|
|[Obter deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Leia as propriedades e as relações do objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|
|[Criar deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Criar um novo objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|
|[Excluir deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|Nenhum|Exclui [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).|
|[Atualizar deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Atualiza as propriedades de um objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário que está sendo relatado em um dispositivo|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado em um dispositivo|
|deviceCount|Int32|Contagem de dispositivos que pertencem a um usuário para uma intenção|
|lastReportedDateTime|DateTimeOffset|Data e hora da última modificação de um relatório de intenção|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Estado do usuário para uma intenção. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```






