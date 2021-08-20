---
title: Tipo de recurso windowsPrivacyDataAccessControlItem
description: Especificar o nível de controle de acesso por categoria de dados de privacidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e69ce442ef3249710b28764cf8b44cebaa3c49e266ea8cae74dacf0cdda9740
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244894"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>Tipo de recurso windowsPrivacyDataAccessControlItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especificar o nível de controle de acesso por categoria de dados de privacidade

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[Coleção windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Listar propriedades e relações dos [objetos windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|
|[Obter windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Leia propriedades e relações do [objeto windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|
|[Criar windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Crie um novo [objeto windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|
|[Excluir windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|Nenhum|Exclui um [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).|
|[Atualizar windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Atualize as propriedades de um [objeto windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave do WindowsPrivacyDataAccessControlItem.|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Isso indica um nível de acesso para a categoria de dados de privacidade ao qual o aplicativo especificado será dado. Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado. Os valores possíveis são: `notConfigured` , , , , , , , , , `accountInfo` , , , , `appsRunInBackground` , , , `calendar` , `callHistory` `camera` , `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` . `syncWithDevices` `trustedDevices`|
|appPackageFamilyName|Cadeia de caracteres|O Nome da Família de Pacotes de um Windows aplicativo. Quando definido, o nível de acesso se aplica ao aplicativo especificado.|
|appDisplayName|Cadeia de caracteres|O Nome da Família de Pacotes de um Windows aplicativo. Quando definido, o nível de acesso se aplica ao aplicativo especificado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```




