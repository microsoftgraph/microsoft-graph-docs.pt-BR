---
title: Tipo de recurso unifiedGroupSource
description: O contêiner do grupo de um custodiado.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b6d1b1d1a7d3abee2516e170fcead20c73235f1f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445942"
---
# <a name="unifiedgroupsource-resource-type"></a>Tipo de recurso unifiedGroupSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner do [grupo de um custodiado.](ediscovery-custodian.md)

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)|[coleção microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Obter uma lista dos **objetos unifiedGroupSource** e suas propriedades.|
|[Criar unifiedGroupSource](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Crie um novo **objeto unifiedGroupSource.**|
|[Obter unifiedGroupSource](../api/ediscovery-unifiedgroupsource-get.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Leia as propriedades e as relações de um **objeto unifiedGroupSource.**|
|[Excluir unifiedGroupSource](../api/ediscovery-unifiedgroupsource-delete.md)|Nenhum(a)|Exclua **um objeto unifiedGroupSource.**|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o unifiedGroupSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o unifiedGroupSource** foi criado.|
|displayName|String|O nome de exibição do grupo unificado - Esse é o nome do grupo.|
|id|String|A ID do **unifiedGroupSource**. Essa não é a ID do grupo real.|
|includedSources|microsoft.graph.ediscovery.sourceType|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|

### <a name="sourcetype-values"></a>valores sourceType

Tipos de fonte relacionados ao usuário. Inclui caixa de correio e site por padrão.

|Member|Descrição|
|:----|-----------|
|mailbox|Representa uma caixa de correio.|
|site|Representa um site do SharePoint.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|group|[group](../resources/group.md)|O grupo associado ao **unifiedGroupSource**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
