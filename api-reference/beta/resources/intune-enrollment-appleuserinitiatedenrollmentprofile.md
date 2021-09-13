---
title: Tipo de recurso appleUserInitiatedEnrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas antes do registro para habilitar o registro de determinados dispositivos cujas identidades foram pré-em estágios. As identidades de dispositivo pré-em estágios são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9fd4060d2f5606326744522e0a9e519714ee28f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081007"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a>Tipo de recurso appleUserInitiatedEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas antes do registro para habilitar o registro de determinados dispositivos cujas identidades foram pré-em estágios. As identidades de dispositivo pré-em estágios são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar appleUserInitiatedEnrollmentProfiles](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|[coleção appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Listar propriedades e relações dos [objetos appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|
|[Obter appleUserInitiatedEnrollmentProfile](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Ler propriedades e relações do [objeto appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|
|[Criar appleUserInitiatedEnrollmentProfile](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Crie um novo [objeto appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|
|[Excluir appleUserInitiatedEnrollmentProfile](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|Nenhum|Exclui um [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).|
|[Atualizar appleUserInitiatedEnrollmentProfile](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Atualize as propriedades de [um objeto appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|
|[Ação setPriority](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultEnrollmentType|[appleUserInitiatedEnrollmentType](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|O tipo de registro de perfil padrão. Os valores possíveis são: `unknown`, `device`, `user`.|
|availableEnrollmentTypeOptions|[Coleção appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)|Lista de opções de tipo de registro disponível|
|id|Cadeia de caracteres|O GUID do objeto.|
|displayName|String|Nome do perfil|
|description|Cadeia de caracteres|Descrição do perfil|
|prioridade|Int32|Prioridade, 0 é mais alta|
|plataforma|[devicePlatformType](../resources/intune-enrollment-deviceplatformtype.md)|A plataforma do Dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|createdDateTime|DateTimeOffset|Tempo de criação de perfil|
|lastModifiedDateTime|DateTimeOffset|Tempo de última modificação do perfil|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)|A lista de atribuições desse perfil.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "String",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "String",
      "enrollmentType": "String"
    }
  ],
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



