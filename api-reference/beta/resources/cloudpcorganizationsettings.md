---
title: Tipo de recurso cloudPcOrganizationSettings
description: Representa as configurações da organização do PC na nuvem para um locatário.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 770531c1d5bcf5dac870b2c341c9b20e2d723e66
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733182"
---
# <a name="cloudpcorganizationsettings-resource-type"></a>Tipo de recurso cloudPcOrganizationSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações da organização do PC na nuvem para um locatário. Um locatário tem apenas um **objeto cloudPcOrganizationSettings** .

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-get.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Leia as propriedades e as relações de um objeto [cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) .|
|[Atualizar cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-update.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Atualize as propriedades de um [objeto cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID das configurações da organização.|
|osVersion|[cloudPcOperatingSystem](#cloudpcoperatingsystem-values)|A versão do sistema operacional (SO) a ser provisionada em PCs na nuvem. Os valores possíveis são: `windows10`, `windows11`, `unknownFutureValue`.|
|userAccountType|[cloudPcUserAccountType](#cloudpcuseraccounttype-values)|O tipo de conta do usuário em PCs na nuvem provisionados. Os valores possíveis são: `standardUser`, `administrator`, `unknownFutureValue`.|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Representa as configurações da organização do PC na nuvem para um locatário. Um locatário tem apenas um **objeto cloudPcOrganizationSettings** . O valor de idioma padrão `en-US`.|

### <a name="cloudpcoperatingsystem-values"></a>Valores de cloudPcOperatingSystem

|Member|Descrição|
|:---|:---|
|windows10|O Windows 10 operacional.|
|windows11|O Windows 11 operacional.|
|unknownFutureValue|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="cloudpcuseraccounttype-values"></a>Valores cloudPcUserAccountType

|Member|Descrição|
|:---|:---|
|standardUser|Um usuário sem permissões administrativas locais no PC na nuvem. Os usuários padrão só podem instalar conteúdo do aplicativo Microsoft Store, mas não podem modificar Windows configurações que exigem privilégios administrativos locais.|
|Administrador|Um usuário com permissões administrativas locais completas no PC na nuvem. Os administradores podem instalar qualquer software e modificar qualquer arquivo ou configuração no PC na nuvem.|
|unknownFutureValue|Valor de sentinel de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOrganizationSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
  "id": "String (identifier)",
  "osVersion": "String",
  "userAccountType": "String",
  "windowsSettings": {
    "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
  }
}
```
