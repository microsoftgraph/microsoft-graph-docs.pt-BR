---
title: Tipo de recurso caseOperation
description: Uma entidade abstrata que representa um processo de execução longa.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 84ea673ad768042ff79f5db0a41fe1d1a4af3e3a
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945065"
---
# <a name="caseoperation-resource-type"></a>Tipo de recurso caseOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Herda de [entidade](../resources/entity.md).

Uma entidade abstrata que representa um processo de Descoberta Eletrônica de execução longa. Ele contém um conjunto comum de propriedades que são compartilhadas entre entidades herdadas.  As entidades que derivam **de caseOperation incluem** :

- [Operação de índice](../resources/security-ediscoveryindexoperation.md)
- [Operação de retenção](../resources/security-ediscoveryholdoperation.md)
- [Limpar operação de dados](../resources/security-ediscoverypurgedataoperation.md)
- [Operação de estimativa](../resources/security-ediscoveryestimateoperation.md)
- [Adicionar à operação de conjunto de revisão](../resources/security-ediscoveryaddtoreviewsetoperation.md)
- [Operação de marca](../resources/security-ediscoverytagoperation.md)
- [Operação de exportação](../resources/security-ediscoveryexportoperation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar caseOperations](../api/security-ediscoverycase-list-operations.md)|[coleção microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Obtenha uma lista dos [objetos caseOperation](../resources/security-caseoperation.md) e suas propriedades.|
|[Obter caseOperation](../api/security-caseoperation-get.md)|[microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Leia as propriedades e as relações de um [objeto caseOperation](../resources/security-caseoperation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,,`convertToPdf`,`estimateStatistics``purgeData`|
|completedDateTime|DateTimeOffset| A data e a hora em que a operação foi concluída. |
|createdBy|[identitySet](../resources/identityset.md)| O usuário que criou a operação. |
|createdDateTime|DateTimeOffset| A data e a hora em que a operação foi criada. |
|id|Cadeia de caracteres| A ID da operação. Somente leitura. |
|percentProgress|Int32| O progresso da operação. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Contém informações de resultado específicas de êxito e falha. |
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="caseaction-values"></a>Valores caseAction

|Member|Descrição|
|:----|-----------|
| addToReviewSet | A operação representa a adição de dados a um conjunto de revisão de uma coleção de Descoberta Eletrônica. |
| applyTags | A operação representa documentos de marcação em massa em um conjunto de revisão para a consulta de conjunto de revisão especificada. |
| contentExport | A operação representa uma exportação de conteúdo de um conjunto de revisão. |
| convertToPdf | A operação representa a conversão de documentos em PDFs com redação. |
| estimateStatistics  | A operação representa a pesquisa em serviços do Microsoft 365, como Exchange, SharePoint e OneDrive for Business. |
| holdUpdate | A operação representa a atualização da retenção legal (aplicar/remover) para custodiantes e fontes de dados não custodiantes.
| index | A operação representa a indexação de fontes de dados de custodiantes e fontes de dados não custodiantes para torná-las pesquisáveis. |
| purgeData | A operação representa a limpeza de conteúdo das cargas de trabalho de origem. |

### <a name="caseoperationstatus-values"></a>Valores caseOperationStatus

|Member|Descrição|
|:----|-----------|
| Notstarted | A operação ainda não foi iniciada. |
| submissionFailed | Falha no envio da operação. |
| Executando | A operação está em execução no momento. |
| Conseguiu | A operação foi concluída com êxito sem erros. |
| partiallySucceeded | A operação foi concluída, mas houve erros - Consulte [resultInfo para](../resources/resultinfo.md) obter detalhes do erro. |
| Falhou | Falha na operação – consulte informações de resultado para obter detalhes do erro. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.caseOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```