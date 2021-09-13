---
title: Tipo de recurso windowsDriverUpdateProfile
description: Windows Perfil de Atualização de Driver
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8837992e47e44dc24a7d49518866d9427d6082e3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029889"
---
# <a name="windowsdriverupdateprofile-resource-type"></a>Tipo de recurso windowsDriverUpdateProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Perfil de Atualização de Driver

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDriverUpdateProfiles](../api/intune-softwareupdate-windowsdriverupdateprofile-list.md)|[Coleção windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Listar propriedades e relações dos [objetos windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Obter windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-get.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Ler propriedades e relações do [objeto windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Criar windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-create.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Crie um novo [objeto windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Excluir windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-delete.md)|Nenhum|Exclui um [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md).|
|[Atualizar windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-update.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Atualize as propriedades de um [objeto windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da política do Intune.|
|displayName|String|O nome de exibição do perfil.|
|description|Cadeia de caracteres|A descrição do perfil especificado pelo usuário.|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|Tipo de aprovação de perfil de atualização de driver. Por exemplo, aprovação manual ou automática. Os valores possíveis são: `manual` e `automatic`.|
|deviceReporting|Int32|Número de dispositivos que relatam esse perfil|
|newUpdates|Int32|Número de novas atualizações de driver disponíveis para esse perfil.|
|deploymentDeferralInDays|Int32|Configurações de adiamento de implantação em dias, aplicável somente quando ApprovalType é definido como aprovação automática.|
|createdDateTime|DateTimeOffset|A data em que o perfil foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data em que o perfil foi modificado pela última vez.|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Lista de Marcas de Escopo para essa entidade de Atualização de Driver.|

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



