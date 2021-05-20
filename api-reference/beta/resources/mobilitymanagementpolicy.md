---
title: Tipo de recurso mobilityManagementPolicy
description: Uma política de gerenciamento de mobilidade representa uma política de registro automático para um aplicativo de gerenciamento de mobilidade configurado no Azure AD.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7f0c073d0737c634872009fffa5425ffe74f4e54
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547320"
---
# <a name="mobilitymanagementpolicy-resource-type"></a>Tipo de recurso mobilityManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Azure AD, uma política de gerenciamento de mobilidade representa uma configuração de registro automático para um aplicativo de gerenciamento de mobilidade (MDM ou MAM). Essas políticas só são aplicáveis a dispositivos com base no sistema operacional Windows 10 e seus derivados (Surface Hub, Hololens etc.). [O registro automático](https://docs.microsoft.com/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal) permite que as organizações registrem automaticamente dispositivos no aplicativo de gerenciamento de mobilidade escolhido como parte do processo de registro do [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-join) ou do [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-register) em Windows 10 dispositivos.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileDeviceManagementPolicies](../api/mobiledevicemanagementpolicies-list.md)|[Coleção mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Obter uma lista dos objetos [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) e suas propriedades para aplicativos de gerenciamento de dispositivo móvel.|
|[Obter mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-get.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Leia as propriedades e as relações de [um objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de dispositivo móvel.|
|[Atualizar mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-update.md)|Nenhum|Atualize as propriedades de [um objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de dispositivo móvel.|
|[Listar includedGroups of mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-list-includedgroups.md)|Coleção [group](../resources/group.md)|Listar grupos incluídos para [um objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de dispositivo móvel.|
|[Adicionar grupo a mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-post-includedgroups.md)|Nenhum|Adicione um grupo ao [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de dispositivo móvel.|
|[Excluir grupo de mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-delete-includedgroups.md)|Nenhum|Exclua um grupo [do objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de dispositivo móvel.|
|[Listar mobileAppManagementPolicies](../api/mobileappmanagementpolicies-list.md)|[Coleção mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Obter uma lista dos objetos [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) e suas propriedades para aplicativos de gerenciamento de aplicativos móveis.|
|[Obter mobileAppManagementPolicy](../api/mobileappmanagementpolicies-get.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Leia as propriedades e as relações de um [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de aplicativo móvel.|
|[Atualizar mobileAppManagementPolicy](../api/mobileappmanagementpolicies-update.md)|Nenhum|Atualize as propriedades de [um objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de aplicativo móvel.|
|[Listar includedGroups of mobileAppManagementPolicy](../api/mobileappmanagementpolicies-list-includedgroups.md)|Coleção [group](../resources/group.md)|Listar grupos incluídos para [um objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de aplicativo móvel.|
|[Adicionar grupo a mobileAppManagementPolicy](../api/mobileappmanagementpolicies-post-includedgroups.md)|Nenhum|Adicione um grupo ao [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de aplicativo móvel.
|[Excluir grupo de mobileAppManagementPolicy](../api/mobileappmanagementpolicies-delete-includedgroups.md)|Nenhum|Exclua um grupo do [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) para um aplicativo de gerenciamento de aplicativo móvel.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appliesTo|policyScope|Indica o escopo do usuário da política de gerenciamento de mobilidade. Os valores possíveis são: `none`, `all`, `selected`.|
|complianceUrl|String|URL de conformidade do aplicativo de gerenciamento de mobilidade.|
|descrição|String|Descrição do aplicativo de gerenciamento de mobilidade.|
|discoveryUrl|String|URL de descoberta do aplicativo de gerenciamento de mobilidade.|
|displayName|String|Nome de exibição do aplicativo de gerenciamento de mobilidade.|
|id|String|ID do objeto do aplicativo de gerenciamento de mobilidade.|
|termsOfUseUrl|String|Termos de Uso URL do aplicativo de gerenciamento de mobilidade.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|includedGroups|Coleção [group](../resources/group.md)|Grupos do Azure AD no escopo do aplicativo de gerenciamento de mobilidade se appliesTo for `selected`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobilityManagementPolicy",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "appliesTo": "String",
  "complianceUrl": "String",
  "description": "String",
  "discoveryUrl": "String",
  "displayName": "String",
  "termsOfUseUrl": "String"
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "mobilityManagementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
