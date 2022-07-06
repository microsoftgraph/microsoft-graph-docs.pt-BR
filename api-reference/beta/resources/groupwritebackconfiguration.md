---
title: Tipo de recurso groupWritebackConfiguration
description: Indica se o write-back de grupos de nuvem para o Active Directory local está habilitado e o tipo de grupo de destino para o grupo local.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 45b14ce9fc0e687c5fbc2cd20fc7b63509d54a0f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645388"
---
# <a name="groupwritebackconfiguration-resource-type"></a>Tipo de recurso groupWritebackConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica se o write-back de grupos de nuvem para o Active Directory local está habilitado e o tipo de grupo de destino para o grupo local.

 Por padrão, todos os Azure AD de segurança não estão habilitados para write-back. Para grupos do Microsoft 365, as configurações padrão definidas pelas propriedades desse recurso podem ser substituídas pelo objeto de `NewUnifiedgroupWritebackDefault` [configuração de diretório](directorysetting.md).

Herda de [writebackConfiguration](../resources/writebackconfiguration.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o write-back de grupos de nuvem para o Active Directory local está habilitado. Anulável. O valor padrão é `true` para grupos do Microsoft 365 e para `false` grupos de segurança. Herdado [de writebackConfiguration](../resources/writebackconfiguration.md).|
|onPremisesGroupType|Cadeia de Caracteres|Indica o tipo de grupo local de destino em que o objeto de nuvem será gravado. Anulável. Os valores possíveis são: `universalDistributionGroup`, `universalSecurityGroup`, `universalMailEnabledSecurityGroup`.<ol><li>Se o grupo de nuvem for um grupo unificado (Microsoft 365), essa propriedade poderá ser uma das seguintes: `universalDistributionGroup`, `universalSecurityGroup`, `universalMailEnabledSecurityGroup`. </li><li>Azure AD grupos de segurança podem ser gravados como `universalSecurityGroup`. </li><li>Se **isEnabled ou** a configuração `NewUnifiedGroupWritebackDefault` [de grupo](directorysetting.md) for `true` , mas essa propriedade não estiver definida explicitamente: <ul><li>Os grupos do Microsoft 365 serão gravados como `universalDistributionGroup` padrão</li></ul><ul><li>Os grupos de segurança serão gravados como `universalSecurityGroup` padrão</li></ul>|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupWritebackConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupWritebackConfiguration",
  "isEnabled": "Boolean",
  "onPremisesGroupType": "String"
}
```

