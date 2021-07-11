---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4b0c0a56fc415c4f2f75ec4972909e31fc9bea14
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366566"
---
# <a name="externalconnection-resource-type"></a>Tipo de recurso externalConnection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner lógico para adicionar conteúdo de uma fonte externa à Microsoft Graph.

## <a name="methods"></a>Métodos

| Método                                                           | Tipo de retorno                                   | Descrição |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Criar externalConnection](../api/external-post-connections.md) | externalConnection                            | Crie um novo externalConnection postando na coleção connections. |
| [Listar externalConnections](../api/externalconnection-list.md)    | Coleção externalConnection                 | Obter uma coleção de objetos externalConnection. |
| [Obter externalConnection](../api/externalconnection-get.md)       | externalConnection                            | Ler propriedades e relações de um objeto externalConnection. |
| [Atualizar externalConnection](../api/externalconnection-update.md) | externalConnection                            | Atualize um objeto externalConnection. |
| [Excluir externalConnection](../api/externalconnection-delete.md) | Nenhum                                          | Exclua um objeto externalConnection. |
| [Criar esquema](../api/externalconnection-post-schema.md)        | Nenhum *ou* [esquema](schema.md)                 | Registrar esquema de conexão. |
| [Obter operação](../api/connectionoperation-get.md)               | [connectionOperation](connectionoperation.md) | Obter o status de uma solicitação assíncrona para criar o esquema de conexão. |
| [Criar externalItem](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | Crie um novo externalItem postando na coleção items. |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição |
|:--------------|:----------------------------------|:------------|
| configuração | [configuration](configuration.md) | Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão. Opcional. |
| descrição   | String                            | Descrição da conexão exibida no Centro de administração do Microsoft 365. Opcional. |
| id            | String                            | ID exclusiva fornecida pelo desenvolvedor da conexão no Azure Active Directory locatário. Comprimento máximo de 32 caracteres. Deve conter somente caracteres alfanuméricos. Não é possível `Microsoft` começar ou ser um dos seguintes valores: , , , `None` , , , , , , , , `Directory` , , `Exchange` , `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` . Obrigatório. |
| nome          | String                            | O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365. Comprimento máximo de 128 caracteres. Obrigatório. |
| state         | connectionState                   | Indica o estado atual da conexão. Os valores possíveis `draft` `ready` são , e `obsolete` `limitExceeded` . Obrigatório. |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                     | Descrição |
|:-------------|:---------------------------------------------------------|:---|
| items        | [Coleção externalItem](externalitem.md)               | Somente leitura. Anulável. |
| operations   | [Coleção connectionOperation](connectionoperation.md) | Somente leitura. Anulável. |
| esquema       | [schema](schema.md)                                      | Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
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
