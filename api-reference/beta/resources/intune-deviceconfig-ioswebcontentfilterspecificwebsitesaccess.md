---
title: tipo de recurso de iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS. Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424760"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>tipo de recurso de iosWebContentFilterSpecificWebsitesAccess

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS. Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.


Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|specificWebsitesOnly|coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|
|websiteList|coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```




