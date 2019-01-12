---
title: tipo de recurso de iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 03e3c4f51e673be1e2bada89e06a26048fe4e385
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916774"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>tipo de recurso de iosWebContentFilterAutoFilter

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





