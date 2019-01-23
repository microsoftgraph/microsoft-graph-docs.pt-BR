---
title: tipo de recurso de iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401226"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>tipo de recurso de iosWebContentFilterAutoFilter

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.


Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedUrls|String collection|URLs adicionais permitidos para o access|
|blockedUrls|String collection|URLs adicionais bloqueados para acesso|

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




