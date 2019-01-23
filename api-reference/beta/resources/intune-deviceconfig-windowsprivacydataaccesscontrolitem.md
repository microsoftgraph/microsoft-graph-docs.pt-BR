---
title: tipo de recurso de windowsPrivacyDataAccessControlItem
description: Especificar o nível de controle de acesso por categoria de dados de privacidade
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a772ab511cd57272da8fb1a3a72a17eb1d06737f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407113"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>tipo de recurso de windowsPrivacyDataAccessControlItem

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Especificar o nível de controle de acesso por categoria de dados de privacidade

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|coleção [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Lista as propriedades e os relacionamentos dos objetos [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|
|[Obter windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Leia as propriedades e os relacionamentos do objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|
|[Criar windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Crie um novo objeto de [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|
|[Excluir windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|Nenhum|Exclui um [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).|
|[Atualizar windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Atualize as propriedades de um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave do WindowsPrivacyDataAccessControlItem.|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Isso indica um nível de acesso para a categoria de dados de privacidade para o qual o aplicativo especificado será fornecido ao. Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Isso indica uma categoria de privacidade de dados ao qual o controle de acesso específico será aplicada. Os valores possíveis são: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .|
|appPackageFamilyName|String|O nome da família de pacote de um aplicativo do Windows. Quando definido, o nível de acesso se aplica ao aplicativo especificado.|
|appDisplayName|String|O nome da família de pacote de um aplicativo do Windows. Quando definido, o nível de acesso se aplica ao aplicativo especificado.|

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




