---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 76fa391d1ce9937bc1799e9bc4ae9470c0794497
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467569"
---
# <a name="externalconnection-resource-type"></a>Tipo de recurso externalConnection

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner lógico para adicionar conteúdo de uma fonte externa à Microsoft Graph.

## <a name="methods"></a>Métodos

| Método                                                           | Tipo de retorno                                   | Descrição |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Criar externalConnection](../api/externalconnectors-external-post-connections.md) | externalConnection                            | Crie um novo externalConnection postando na coleção connections. |
| [Listar externalConnections](../api/externalconnectors-externalconnection-list.md)    | Coleção externalConnection                 | Obter uma coleção de objetos externalConnection. |
| [Obter externalConnection](../api/externalconnectors-externalconnection-get.md)       | externalConnection                            | Ler propriedades e relações de um objeto externalConnection. |
| [Atualizar externalConnection](../api/externalconnectors-externalconnection-update.md) | externalConnection                            | Atualize um objeto externalConnection. |
| [Excluir externalConnection](../api/externalconnectors-externalconnection-delete.md) | Nenhum                                          | Exclua um objeto externalConnection. |
| [Criar esquema](../api/externalconnectors-externalconnection-post-schema.md)        | Nenhum *ou* [esquema](externalconnectors-schema.md)                 | Registrar esquema de conexão. |
| [Obter operação](../api/externalconnectors-connectionoperation-get.md)               | [connectionOperation](externalconnectors-connectionoperation.md) | Obter o status de uma solicitação assíncrona para criar o esquema de conexão. |
| [Criar externalItem](../api/externalconnectors-externalconnection-put-items.md)    | [externalItem](externalconnectors-externalitem.md)               | Crie um novo externalItem postando na coleção items. |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição |
|:--------------|:----------------------------------|:------------|
| configuração | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão. Opcional. |
| description   | String                            | Descrição da conexão exibida no Centro de administração do Microsoft 365. Opcional. |
| id            | String                            | ID exclusiva fornecida pelo desenvolvedor da conexão no Azure Active Directory locatário. Deve ter entre 3 e 32 caracteres de comprimento. Deve conter somente caracteres alfanuméricos. Não é possível começar ou ser um dos `Microsoft` seguintes valores: `None` , , , , , , , , `Directory` , , , , `Exchange` , , `ExchangeArchive` , `LinkedIn` , `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` . `MSFT_All_Connectors` Obrigatório. |
| nome          | String                            | O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365. Comprimento máximo de 128 caracteres. Obrigatório. |
| state         | microsoft.graph.externalConnectors.connectionState                   | Indica o estado atual da conexão. Os valores possíveis `draft` `ready` são , e `obsolete` `limitExceeded` . Obrigatório. |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                     | Descrição |
|:-------------|:---------------------------------------------------------|:---|
| items        | [Coleção microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)               | Somente leitura. Anulável. |
| operations   | [coleção microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) | Somente leitura. Anulável. |
| schema       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "keyProperty": "id"
}-->

```json
{
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
