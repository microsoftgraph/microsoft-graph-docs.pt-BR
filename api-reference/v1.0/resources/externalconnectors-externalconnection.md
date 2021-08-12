---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: beb0a9b424f1207a7cf378e6bbb17c747ca68ca50617381766ee4dc8d5232828
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180856"
---
# <a name="externalconnection-resource-type"></a>Tipo de recurso externalConnection

Namespace: microsoft.graph.externalConnectors

Um contêiner lógico para adicionar conteúdo de uma fonte externa à Microsoft Graph.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalConnection](../api/externalconnectors-external-post-connections.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|Crie um novo [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Listar externalConnections](../api/externalconnectors-externalconnection-list.md)|[Coleção externalConnection](../resources/externalconnectors-externalconnection.md)|Obter uma lista dos [objetos externalConnection](../resources/externalconnectors-externalconnection.md) e suas propriedades.|
|[Obter externalConnection](../api/externalconnectors-externalconnection-get.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|Leia as propriedades e as relações de um [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Atualizar externalConnection](../api/externalconnectors-externalconnection-update.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|Atualize as propriedades de [um objeto externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Excluir externalConnection](../api/externalconnectors-externalconnection-delete.md)|None|Exclui um [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Criar esquema](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|Crie um novo objeto de esquema.|
|[Criar externalItem](../api/externalconnectors-externalitem-create.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Crie um novo objeto externalItem.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configuração|[microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md)|Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão. Opcional.|
|description|Cadeia de caracteres|Descrição da conexão exibida no Centro de administração do Microsoft 365. Opcional.|
|id|Cadeia de caracteres| ID exclusiva fornecida pelo desenvolvedor da conexão no Azure Active Directory locatário. Deve ter entre 3 e 32 caracteres de comprimento. Deve conter somente caracteres alfanuméricos. Não é possível começar ou ser um dos `Microsoft` seguintes valores: `None` , , , , , , , , `Directory` , , , , `Exchange` , , `ExchangeArchive` , `LinkedIn` , `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` . `MSFT_All_Connectors` Obrigatório. |
|nome|String|O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365. Comprimento máximo de 128 caracteres. Obrigatório.|
|state|microsoft.graph.externalConnectors.connectionState|Indica o estado atual da conexão. Os valores possíveis são: `draft`, `ready`, `obsolete`, `limitExceeded`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|items|[Coleção microsoft.graph.externalConnectors.externalItem](../resources/externalconnectors-externalitem.md)|Somente leitura. Anulável.|
|operations|[coleção microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md)|Somente leitura. Anulável.|
|schema|[microsoft.graph.externalConnectors.schema](../resources/externalconnectors-schema.md)|Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "state": "String"
}
```

