---
title: tipo de recurso diário
description: Um diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bef5008bbacb1729f48758b228e55a3f6adc2af0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365469"
---
# <a name="journal-resource-type"></a>tipo de recurso diário
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
|displayName         |Cadeia de caracteres, tamanho máximo 50| O nome de exibição do diário.                     |
|lastModifiedDateTime|DateTime               |O último DateTime que o diário foi modificado. Somente Leitura.|

## <a name="bound-actions"></a>Ações associadas
O tipo de recurso diário oferece uma ação associada `post` chamada que envia o lote de diário geral correspondente.

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

