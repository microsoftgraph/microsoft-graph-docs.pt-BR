---
title: tipo de recurso externalConnection
description: Uma conexão com a Microsoft Search a partir de uma fonte externa.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a5db824fabc1cedb27d15c4b2cbfbce08bd59191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026926"
---
# <a name="externalconnection-resource-type"></a>tipo de recurso externalConnection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma conexão com a Microsoft Search a partir de uma fonte externa.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método                                                           | Tipo de retorno                                   | Descrição |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Criar externalConnection](../api/external-post-connections.md) | externalConnection                            | Crie um novo externalConnection postando na coleção Connections. |
| [Listar externalConnections](../api/externalconnection-list.md)    | coleção externalConnection                 | Obtenha uma coleção de objetos externalConnection. |
| [Obter externalConnection](../api/externalconnection-get.md)       | externalConnection                            | Ler propriedades e relações de um objeto externalConnection. |
| [Atualizar externalConnection](../api/externalconnection-update.md) | externalConnection                            | Atualizar um objeto externalConnection. |
| [Excluir externalConnection](../api/externalconnection-delete.md) | Nenhum                                          | Excluir um objeto externalConnection. |
| [Criar esquema](../api/externalconnection-post-schema.md)        | Nenhum *ou* [esquema](schema.md)                 | Registrar o esquema de conexão. |
| [Operação get](../api/connectionoperation-get.md)               | [connectionOperation](connectionoperation.md) | Obter o status de uma solicitação assíncrona para criar o esquema de conexão. |
| [Criar externalItem](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | Criar um novo externalItem postando na coleção Items. |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição |
|:--------------|:----------------------------------|:------------|
| configuration | [configuration](configuration.md) | Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão. Opcional. |
| description   | String                            | Descrição da conexão exibida no centro de administração do Microsoft 365. Opcional. |
| id            | String                            | ID exclusiva fornecida pelo desenvolvedor da conexão dentro do locatário do Azure Active Directory. Comprimento máximo de 32 caracteres. Deve conter apenas caracteres alfanuméricos. Não pode começar com `Microsoft` um dos seguintes valores:,, `None` `Directory` ,, `Exchange` `ExchangeArchive` `LinkedIn` , `Mailbox` , `MicrosoftSearch` , `OneDriveBusiness` ,,, `SharePoint` , `Teams` `Yammer` `Connectors` ,,,,,,,,,. Obrigatório. |
| nome          | String                            | O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365. Comprimento máximo de 128 caracteres. Obrigatório. |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                     | Descrição |
|:-------------|:---------------------------------------------------------|:---|
| items        | coleção [externalItem](externalitem.md)               | Somente leitura. Anulável. |
| operations   | coleção [connectionOperation](connectionoperation.md) | Somente leitura. Anulável. |
| esquemas       | [schema](schema.md)                                      | Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


