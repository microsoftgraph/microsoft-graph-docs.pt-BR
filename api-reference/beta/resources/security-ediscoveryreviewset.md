---
title: Tipo de recurso ediscoveryReviewSet
description: Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em um litígio, investigação ou solicitação regulatória.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 130f274e9bb9bff1eb2e573366bba3fbe8d4ed77
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838609"
---
# <a name="ediscoveryreviewset-resource-type"></a>Tipo de recurso ediscoveryReviewSet

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em um litígio, investigação ou solicitação regulatória.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryReviewSets](../api/security-ediscoverycase-list-reviewsets.md)|[coleção microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Obtenha uma lista dos [objetos ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) e suas propriedades.|
|[Criar ediscoveryReviewSet](../api/security-ediscoverycase-post-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Crie um novo [objeto ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) .|
|[Obter ediscoveryReviewSet](../api/security-ediscoveryreviewset-get.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Leia as propriedades e as relações de um [objeto ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) .|
|[Exportação](../api/security-ediscoveryreviewset-export.md)|Nenhum|Inicie uma exportação de dados de um conjunto [de revisão](../resources/security-ediscoveryreviewset.md).|
|[addToReviewSet](../api/security-ediscoveryreviewset-addtoreviewset.md)|Nenhum|Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um [conjunto de revisão](../resources/security-ediscoveryreviewset.md).|
|[Listar arquivos](../api/security-ediscoveryreviewset-list-files.md)|[coleção microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Obtenha os recursos de ediscoveryFile da propriedade de navegação de arquivos.|
|[Listar consultas](../api/security-ediscoveryreviewset-list-queries.md)|[coleção microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Obtenha a lista [de consultas associadas](../resources/security-ediscoveryreviewsetquery.md) a um conjunto de revisão de Descoberta Eletrônica.|
|[Criar ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-post-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Crie um novo objeto ediscoveryReviewSetQuery.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](../resources/identityset.md)|O usuário que criou o conjunto de revisão. Somente leitura. |
|createdDateTime|DateTimeOffset|O datetime em que o conjunto de revisão foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do conjunto de revisão. O nome é exclusivo com um limite máximo de 64 caracteres.|
|id|String|O identificador exclusivo do conjunto de revisão. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|arquivos|[coleção microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Representa arquivos dentro do conjunto de revisão.|
|Consultas|[coleção microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Representa consultas dentro do conjunto de revisão.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewSet",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)"
}
```

