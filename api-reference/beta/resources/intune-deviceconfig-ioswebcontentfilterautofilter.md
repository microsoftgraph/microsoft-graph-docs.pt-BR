---
title: tipo de recurso de iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.
ms.openlocfilehash: 04a221ac512ab3934702a2a9e3178ba23a2ac3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038744"
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





