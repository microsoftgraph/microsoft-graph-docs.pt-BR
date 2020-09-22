---
title: tipo de recurso countriesRegions
description: Um objeto de países/regiões no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 490fa240cda525b517bf4e8dcec3e89aedbcc201
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049805"
---
# <a name="countriesregions-resource-type"></a>tipo de recurso countriesRegions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto countriesRegions no Dynamics 365 Business central, que é parte de um endereço.

## <a name="methods"></a>Métodos

| Método                                                              | Tipo de retorno    |Descrição                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[Obter countriesRegions](../api/dynamics-countriesregions-get.md)      |countriesRegions|Obter um país/região.   |
|[Postar countriesRegions](../api/dynamics-create-countriesregions.md)  |countriesRegions|Criar um país/região.|
|[Patch countriesRegions](../api/dynamics-countriesregions-update.md) |countriesRegions|Atualize um país/região.|
|[Excluir countriesRegions](../api/dynamics-countriesregions-delete.md)|Nenhuma            |Exclua os países/regiões.|

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo       |Descrição                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|id              |GUID        |A identificação exclusiva do país/região. Não editável.           |
|código            |cadeia de caracteres      |Especifica o código do país/região.                    |
|displayName     |cadeia de caracteres      |Especifica o nome de exibição do país/região.            |
|addressFormat   |cadeia de caracteres      |Especifica o formato do endereço exibido em documentos de face externa. Você vincula um formato de endereço a um código de país/região para que documentos externos baseados em cartões ou documentos com esse código de país/região usem o formato de endereço especificado.|
|lastModifiedDateTime|datetime|O último DateTime que o país/região foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do countriesRegions.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```




