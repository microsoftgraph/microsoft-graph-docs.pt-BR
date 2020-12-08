---
title: tipo de recurso unifiedGroupSource
description: O contêiner para o grupo de um dos responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 5fba2a994cda61f111739d98ea3a210c76ffeb23
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597525"
---
# <a name="unifiedgroupsource-resource-type"></a>tipo de recurso unifiedGroupSource

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner para o grupo de um [dos responsáveis](custodian.md) .

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|coleção [unifiedGroupSource](../resources/unifiedgroupsource.md)|Obtenha uma lista dos objetos **unifiedGroupSource** e suas propriedades.|
|[Criar unifiedGroupSource](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|Criar um novo objeto **unifiedGroupSource** .|
|[Obter unifiedGroupSource](../api/unifiedgroupsource-get.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|Leia as propriedades e os relacionamentos de um objeto **unifiedGroupSource** .|
|[Excluir unifiedGroupSource](../api/unifiedgroupsource-delete.md)|Nenhum|Excluir um objeto **unifiedGroupSource** .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou o **unifiedGroupSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em que o **unifiedGroupSource** foi criado.|
|displayName|String|O nome de exibição do grupo unificado-este é o nome do grupo.|
|id|String|A ID do **unifiedGroupSource**. Essa não é a ID do grupo real.|
|includedSources|sourceType|Especifica quais fontes são incluídas nesse grupo. Os valores possíveis são: `mailbox` e `site`.|

### <a name="sourcetype-values"></a>valores de sourceType

Tipos de fonte relacionados ao usuário. Inclui a caixa de correio e o site por padrão.

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
  "@odata.type": "microsoft.graph.unifiedGroupSource",
  "baseType": "microsoft.graph.dataSource",
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
