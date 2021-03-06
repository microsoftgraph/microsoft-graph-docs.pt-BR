---
title: tipo de recurso diário
description: Um diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ecbeba91828ba06b9927af08ac8d75a177e27cea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013829"
---
# <a name="journal-resource-type"></a>tipo de recurso diário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um diário no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método                                            |Tipo de retorno|Descrição    |
|:--------------------------------------------------|:----------|:--------------|
|[Obter diário](../api/dynamics-journal-get.md)      |diário    |Obtém um diário.   |
|[Diário de lançamentos](../api/dynamics-create-journal.md)  |diário    |Cria um diário.|
|[Diário de patches](../api/dynamics-journal-update.md) |diário    |Atualiza um diário.|
|[Excluir diário](../api/dynamics-journal-delete.md)|Nenhuma       |Exclui um diário.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|id                  |GUID                   |A ID exclusiva do diário. Não editável.           |
|código                |Cadeia de caracteres, tamanho máximo 10| O código do diário.                             |
|Nome para exibição         |Cadeia de caracteres, tamanho máximo 50| O nome de exibição do diário.                     |
|lastModifiedDateTime|datetime               |O último DateTime que o diário foi modificado. Somente Leitura.|

## <a name="bound-actions"></a>Ações associadas
O tipo de recurso diário oferece uma ação associada chamada `post` que envia o lote de diário geral correspondente.

O lançamento do lote de diário geral é ilustrado no exemplo a seguir:  
`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.

A resposta não tem conteúdo; o código de resposta é 204.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```



