---
title: Tipo de recurso windowsFeatureUpdateProfile
description: Perfil de Atualização de Recursos do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea8ead87af7e1f0b968ee9b85aaf0b7b4efbbcb6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133385"
---
# <a name="windowsfeatureupdateprofile-resource-type"></a>Tipo de recurso windowsFeatureUpdateProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de Atualização de Recursos do Windows

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsFeatureUpdateProfiles](../api/intune-softwareupdate-windowsfeatureupdateprofile-list.md)|[Coleção windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Listar propriedades e relações dos [objetos windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Obter windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-get.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Leia propriedades e relações do [objeto windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Criar windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-create.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Crie um novo [objeto windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Excluir windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|Nenhum|Exclui um [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).|
|[Atualizar windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Atualize as propriedades de um [objeto windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[atribuir ação](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O Identificador da entidade.|
|displayName|Cadeia de caracteres|O nome de exibição do perfil.|
|descrição|Cadeia de caracteres|A descrição do perfil especificado pelo usuário.|
|featureUpdateVersion|Cadeia de caracteres|A versão de atualização de recursos que será implantada nos dispositivos direcionados por esse perfil. A versão pode ser qualquer versão com suporte para o exemplo 1709, 1803 ou 1809 e assim por diante.|
|createdDateTime|DateTimeOffset|A data em que o perfil foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data em que o perfil foi modificado pela última vez.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de Marcas de Escopo para essa entidade atualização de recursos.|
|deployableContentDisplayName|Cadeia de caracteres|Nome de exibição amigável do conteúdo implantável do perfil de atualização de qualidade|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|A lista de atribuições de grupo do perfil.|
|deviceUpdateStates|[Coleção windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|A lista de dispositivos declara esse perfil direcionado para|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "featureUpdateVersion": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "deployableContentDisplayName": "String"
}
```




