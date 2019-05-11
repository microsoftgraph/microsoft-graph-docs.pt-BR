---
title: tipo de recurso iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6bf2da4320c228123e24ae67bd21b13f2c21eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946067"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>tipo de recurso iosWebContentFilterAutoFilter

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.


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




