---
title: tipo de recurso de contas
description: Um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 671d81da52b28558fa5c24b13060b766c8d908c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076453"
---
# <a name="accounts-resource-type"></a>tipo de recurso de contas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto Account no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contas](../api/dynamics-account-get.md)|contas|Obtém o objeto accounts.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A identificação exclusiva da conta.|
|number|Cadeia de caracteres, tamanho máximo 20|Especifica o número da conta G/L.|
|displayName|Cadeia de caracteres, tamanho máximo 50|Especifica o nome da conta de G/L.|
|category|Cadeia de caracteres, tamanho máximo 20|Especifica a categoria da conta de G/L.|
|Subcategoria|Cadeia de caracteres, tamanho máximo 80|Especifica a subcategoria da categoria de conta da conta G/L.|
|bloqueou|booliano|Especifica que não é possível postar entradas na conta G/L. **True** indica que a conta está bloqueada e o lançamento não é permitido.|
|lastModifiedDateTime|datetime|O último DateTime que a conta foi modificada.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}
```


