---
title: Tipo de recurso iosWebContentFilterAutoFilter
description: Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que habilita o recurso de filtro automático do iOS e permite um controle de acesso de URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cbd15f366397564b24f6c715eaf2ea9b6826d30
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58813002"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Tipo de recurso iosWebContentFilterAutoFilter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que habilita o recurso de filtro automático do iOS e permite um controle de acesso de URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.


Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedUrls|Coleção de cadeias de caracteres|URLs adicionais permitidas para acesso|
|blockedUrls|Coleção de cadeias de caracteres|URLs adicionais bloqueadas para acesso|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```



