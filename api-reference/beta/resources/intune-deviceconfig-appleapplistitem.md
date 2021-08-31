---
title: Tipo de recurso appleAppListItem
description: Representa um aplicativo na lista de aplicativos da Apple gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2111e8e8403b312c17a7c9e2c6dad62c857d4282
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796261"
---
# <a name="appleapplistitem-resource-type"></a>Tipo de recurso appleAppListItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um aplicativo na lista de aplicativos da Apple gerenciados


Herda de [appListItem](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|O nome do aplicativo Herdado do [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|publicador|String|O editor do aplicativo Herdado do [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appStoreUrl|String|A URL da Loja do aplicativo Herdado do [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appId|Cadeia de caracteres|O identificador de aplicativo ou pacote do aplicativo Herdado do [appListItem](../resources/intune-deviceconfig-applistitem.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



