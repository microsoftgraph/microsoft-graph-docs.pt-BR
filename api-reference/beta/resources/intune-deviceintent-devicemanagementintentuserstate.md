---
title: Tipo de recurso deviceManagementIntentUserState
description: Entidade que representa o estado do usuário para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd683b76a2641e9b3df6b7caee3e98fece063a3f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796219"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>Tipo de recurso deviceManagementIntentUserState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o estado do usuário para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentUserStates](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|[Coleção deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Listar propriedades e relações dos [objetos deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|
|[Obter deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Ler propriedades e relações do [objeto deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|
|[Criar deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Crie um novo [objeto deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|
|[Excluir deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|Nenhum(a)|Exclui um [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).|
|[Atualizar deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Atualize as propriedades de [um objeto deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário que está sendo relatado em um dispositivo|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado em um dispositivo|
|deviceCount|Int32|Contagem de dispositivos que pertencem a um usuário para uma intenção|
|lastReportedDateTime|DateTimeOffset|Data da última modificação de um relatório de intenção|
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



