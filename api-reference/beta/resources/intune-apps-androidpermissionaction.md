---
title: tipo de recurso androidPermissionAction
description: O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce351edc83ac31c21c05b7d3e64c2f3be315da61
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799259"
---
# <a name="androidpermissionaction-resource-type"></a>tipo de recurso androidPermissionAction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|autorização|String|Cadeia de caracteres de permissão Android, definida na documentação oficial do Android.  Exemplo ' Android. Permission. READ_CONTACTS '.|
|ação|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Tipo de ação de permissão de Android. Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```



