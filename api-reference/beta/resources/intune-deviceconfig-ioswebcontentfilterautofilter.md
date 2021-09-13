---
title: Tipo de recurso iosWebContentFilterAutoFilter
description: Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que habilita o recurso de filtro automático do iOS e permite um controle de acesso de URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c88850a9cb9cfab27da02231a908ed9466b6389
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127231"
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
|allowedUrls|String collection|URLs adicionais permitidas para acesso|
|blockedUrls|String collection|URLs adicionais bloqueadas para acesso|

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



