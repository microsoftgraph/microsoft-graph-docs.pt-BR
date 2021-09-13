---
title: Tipo de recurso androidPermissionAction
description: Mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve tomar quando essa permissão for solicitada.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1065497839de4ccc4a90d48deb6651e11422e84
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115601"
---
# <a name="androidpermissionaction-resource-type"></a>Tipo de recurso androidPermissionAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve tomar quando essa permissão for solicitada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|permission|Cadeia de Caracteres|Cadeia de caracteres de permissão do Android, definida na documentação oficial do Android.  Exemplo 'android.permission.READ_CONTACTS'.|
|ação|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Tipo de ação de permissão do Android. Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.|

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



