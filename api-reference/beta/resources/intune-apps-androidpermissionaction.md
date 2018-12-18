---
title: tipo de recurso de androidPermissionAction
description: Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.
author: tfitzmac
ms.openlocfilehash: 90117b30dae765151e79d8ad1c2ae1afaa5a42ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331133"
---
# <a name="androidpermissionaction-resource-type"></a>tipo de recurso de androidPermissionAction

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|permissão|String|String de permissão Android, definido na documentação oficial Android.  Exemplo 'android.permission.READ_CONTACTS'.|
|action|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Tipo de ação de permissão Android. Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.|

## <a name="relationships"></a>Relacionamentos
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





