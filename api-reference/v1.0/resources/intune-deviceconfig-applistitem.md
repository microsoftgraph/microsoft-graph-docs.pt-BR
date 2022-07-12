---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02efd729349e709fe06f0d1cdcd621dece95732e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730998"
---
# <a name="applistitem-resource-type"></a>Tipo de recurso appListItem

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um aplicativo na lista de aplicativos gerenciados

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|O nome do aplicativo|
|distribuidor|Cadeia de caracteres|O distribuidor do aplicativo|
|appStoreUrl|Cadeia de caracteres|A URL da loja do aplicativo|
|appId|String|O aplicativo ou identificador do pacote do aplicativo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





