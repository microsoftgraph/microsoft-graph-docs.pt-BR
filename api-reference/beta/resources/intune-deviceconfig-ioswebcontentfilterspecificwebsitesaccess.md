---
title: Tipo de recurso iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que instala indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula onde os professores gostaria que os alunos navegam em sites por meio de indicadores do navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b167caad8dac1ec98771398f68f217c288d5a0557c4342a5d8f32ee9009486c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54127128"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>Tipo de recurso iosWebContentFilterSpecificWebsitesAccess

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que instala indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula onde os professores gostaria que os alunos navegam em sites por meio de indicadores do navegador configurados em seus dispositivos iOS e sem acesso a outros sites.


Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|specificWebsitesOnly|[Coleção iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Os indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|
|websiteList|[Coleção iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Os indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|

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




