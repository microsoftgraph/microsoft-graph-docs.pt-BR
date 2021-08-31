---
title: Tipo de recurso windowsQualityUpdateProfile
description: Windows Perfil de Atualização de Qualidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 247b382ec9d12c621591a9efcd1a6904005a7f3d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797469"
---
# <a name="windowsqualityupdateprofile-resource-type"></a>Tipo de recurso windowsQualityUpdateProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Perfil de Atualização de Qualidade

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsQualityUpdateProfiles](../api/intune-softwareupdate-windowsqualityupdateprofile-list.md)|[Coleção windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Listar propriedades e relações dos objetos [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Obter windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-get.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Leia propriedades e relações do [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Criar windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-create.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Crie um novo [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Excluir windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-delete.md)|Nenhum(a)|Exclui um [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).|
|[Atualizar windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-update.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Atualize as propriedades de um [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[atribuir ação](../api/intune-softwareupdate-windowsqualityupdateprofile-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da política do Intune.|
|displayName|Cadeia de caracteres|O nome de exibição do perfil.|
|descrição|Cadeia de caracteres|A descrição do perfil especificado pelo usuário.|
|expeditedUpdateSettings|[expeditedWindowsQualityUpdateSettings](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|Configurações de atualização aceleradas.|
|createdDateTime|DateTimeOffset|A data em que o perfil foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data em que o perfil foi modificado pela última vez.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de Marcas de Escopo para esta entidade de Atualização de Qualidade.|
|releaseDateDisplayName|Cadeia de caracteres|Data de lançamento amigável a ser exibida para um lançamento de Atualização de Qualidade|
|deployableContentDisplayName|Cadeia de caracteres|Nome de exibição amigável do conteúdo implantável do perfil de atualização de qualidade|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|A lista de atribuições de grupo do perfil.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "String",
    "daysUntilForcedReboot": 1024
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "releaseDateDisplayName": "String",
  "deployableContentDisplayName": "String"
}
```



