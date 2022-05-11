---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 417af041fc70ce86e921568b60059948754b942f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315696"
---
# <a name="externalconnection-resource-type"></a>Tipo de recurso externalConnection

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner lógico para adicionar conteúdo de uma fonte externa ao Microsoft Graph.

## <a name="methods"></a>Métodos

| Método                                                           | Tipo de retorno                                   | Descrição |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Criar externalConnection](../api/externalconnectors-external-post-connections.md) | externalConnection                            | Crie um novo **externalConnection** postando na coleção de conexões. |
| [Listar externalConnections](../api/externalconnectors-externalconnection-list.md)    | coleção externalConnection                 | Obtenha uma **coleção de objetos externalConnection** . |
| [Obter externalConnection](../api/externalconnectors-externalconnection-get.md)       | externalConnection                            | Ler propriedades e relações de um **objeto externalConnection** . |
| [Atualizar externalConnection](../api/externalconnectors-externalconnection-update.md) | externalConnection                            | Atualize **um objeto externalConnection** . |
| [Excluir externalConnection](../api/externalconnectors-externalconnection-delete.md) | Nenhum                                          | **Exclua um objeto externalConnection**. |
| [Criar esquema](../api/externalconnectors-externalconnection-post-schema.md)        | Nenhum *ou* [esquema](externalconnectors-schema.md)                 | Registrar esquema de conexão. |
| [Obter operação](../api/externalconnectors-connectionoperation-get.md)               | [connectionOperation](externalconnectors-connectionoperation.md) | Obtenha o status de uma solicitação assíncrona para criar o esquema de conexão. |
| [Criar externalItem](../api/externalconnectors-externalconnection-put-items.md)    | [externalItem](externalconnectors-externalitem.md)               | Crie um novo externalItem postando na coleção de itens. |
|[Obter connectionQuota](../api/externalconnectors-connectionquota-get.md)|[connectionQuota](../resources/externalconnectors-connectionquota.md)| Recupere as propriedades e as relações de uma **connectionQuota**. |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição |
|:--------------|:----------------------------------|:------------|
| configuração | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão. Opcional. |
| connectorId   |Cadeia de caracteres                             | A Teams ID do aplicativo. Opcional.|
| description   | Cadeia de caracteres                            | Descrição da conexão exibida no Centro de administração do Microsoft 365. Opcional. |
| id            | String                            | ID exclusiva fornecida pelo desenvolvedor da conexão dentro do Azure Active Directory locatário. Deve ter entre 3 e 32 caracteres. Deve conter apenas caracteres alfanuméricos. Não é possível começar `Microsoft` com ou ser um dos seguintes valores: `None`, `Directory`, , `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`, `TaskFabric`, `PowerBI`, `Assistant`, `TopicEngine``MSFT_All_Connectors`. Obrigatório. |
| ingestedItemsCount           | Int64                            |  O número de itens ingeridos em uma conexão. Esse valor é atualizado a cada 15 minutos. Se o estado de conexão for `draft`, **ingestedItemsCount** será `null`. |
| nome          | String                            | O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365. Comprimento máximo de 128 caracteres. Obrigatório. |
| searchSettings|[microsoft.graph.externalConnectors.searchSettings](../resources/externalconnectors-searchsettings.md)|As configurações que definem a experiência de pesquisa para conteúdo nessa conexão, como os modelos de exibição para resultados da pesquisa.|
| estado         | microsoft.graph.externalConnectors.connectionState                   | Indica o estado atual da conexão. Os valores possíveis `draft`são `ready`, `obsolete`e `limitExceeded`. Obrigatório. |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                     | Descrição |
|:-------------|:---------------------------------------------------------|:---|
| grupos       | [Coleção microsoft.graph.externalConnectors.externalGroup](externalconnectors-externalgroup.md)             | Somente leitura. Anulável. |
| items        | [Coleção microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)               | Somente leitura. Anulável. |
| operations   | [Coleção microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) | Somente leitura. Anulável. |
| quota        | [microsoft.graph.externalConnectors.connectionQuota](externalconnectors-connectionquota.md)             | Somente leitura. Anulável. |
| Esquema       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | Somente leitura. Anulável. |

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
  "ingestedItemsCount": "Int64",
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
