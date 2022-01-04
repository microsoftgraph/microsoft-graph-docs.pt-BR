---
title: Tipo de recurso windowsDriverUpdateProfile
description: Windows de atualização de driver
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee9304666ac2bc71485e25f8de16decc5c4d10fc
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712093"
---
# <a name="windowsdriverupdateprofile-resource-type"></a>Tipo de recurso windowsDriverUpdateProfile

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows de atualização de driver

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDriverUpdateProfiles](../api/intune-softwareupdate-windowsdriverupdateprofile-list.md)|[Coleção windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Listar propriedades e relações dos [objetos windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Obter windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-get.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Ler propriedades e relações do [objeto windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Criar windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-create.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Crie um novo [objeto windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Excluir windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-delete.md)|Nenhum|Exclui um [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md).|
|[Atualizar windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-update.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Atualize as propriedades de um [objeto windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[atribuir ação](../api/intune-softwareupdate-windowsdriverupdateprofile-assign.md)|Nenhuma|Ainda não documentado|
|[Ação executeAction](../api/intune-softwareupdate-windowsdriverupdateprofile-executeaction.md)|[bulkDriverActionResult](../resources/intune-softwareupdate-bulkdriveractionresult.md)|Ainda não documentado|
|[Ação syncInventory](../api/intune-softwareupdate-windowsdriverupdateprofile-syncinventory.md)|Nenhum|Sincronizar o inventário de driver de um WindowsDriverUpdateProfile.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da política do Intune.|
|displayName|String|O nome de exibição do perfil.|
|descrição|String|A descrição do perfil especificado pelo usuário.|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|Tipo de aprovação de perfil de atualização de driver. Por exemplo, aprovação manual ou automática. Os valores possíveis são: `manual` e `automatic`.|
|deviceReporting|Int32|Número de dispositivos que relatam esse perfil|
|newUpdates|Int32|Número de novas atualizações de driver disponíveis para esse perfil.|
|deploymentDeferralInDays|Int32|Configurações de adiamento de implantação em dias, aplicável somente quando ApprovalType é definido como aprovação automática.|
|createdDateTime|DateTimeOffset|A data em que o perfil foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data em que o perfil foi modificado pela última vez.|
|roleScopeTagIds|Coleção String|Lista de Marcas de Escopo para essa entidade de Atualização de Driver.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|A lista de atribuições de grupo do perfil.|
|driverInventories|[Coleção windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Inventários de driver para esse perfil.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "approvalType": "String",
  "deviceReporting": 1024,
  "newUpdates": 1024,
  "deploymentDeferralInDays": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




