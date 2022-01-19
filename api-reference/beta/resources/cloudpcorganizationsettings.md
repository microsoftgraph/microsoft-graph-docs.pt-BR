---
title: Tipo de recurso cloudPcOrganizationSettings
description: Representa as configurações da organização do computador na nuvem para um locatário.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0a74f5db7c98cf5f6ec96d1fbddb5908f28ccea5
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072780"
---
# <a name="cloudpcorganizationsettings-resource-type"></a>Tipo de recurso cloudPcOrganizationSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações da organização do computador na nuvem para um locatário. Um locatário tem apenas um **objeto cloudPcOrganizationSettings.**

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-get.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Leia as propriedades e as relações de um [objeto cloudPcOrganizationSettings.](../resources/cloudpcorganizationsettings.md)|
|[Atualizar cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-update.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Atualize as propriedades de [um objeto cloudPcOrganizationSettings.](../resources/cloudpcorganizationsettings.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID das configurações da organização.|
|osVersion|[cloudPcOperatingSystem](#cloudpcoperatingsystem-values)|O tipo de conta do usuário em PCs de Nuvem provisionados. Os valores possíveis são: `windows10`, `windows11`, `unknownFutureValue`.|
|userAccountType|[cloudPcUserAccountType](#cloudpcuseraccounttype-values)|A versão do sistema operacional (OS) a ser provisionada em PCs na Nuvem. Os valores possíveis são: `standardUser`, `administrator`, `unknownFutureValue`.|

### <a name="cloudpcoperatingsystem-values"></a>Valores do cloudPcOperatingSystem

|Member|Descrição|
|:---|:---|
|windows10|O Windows 10 operacional.|
|windows11|O Windows 11.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="cloudpcuseraccounttype-values"></a>valores cloudPcUserAccountType

|Member|Descrição|
|:---|:---|
|standardUser|Um usuário sem permissões administrativas locais no Cloud PC. Os usuários padrão só podem instalar conteúdo do aplicativo Microsoft Store, mas não podem modificar Windows configurações que exigem privilégios administrativos locais.|
|administrator|Um usuário com permissões administrativas locais completas no Cloud PC. Os administradores podem instalar qualquer software e modificar qualquer arquivo ou configuração no Cloud PC.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

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
  "userAccountType": "String"
}
```
