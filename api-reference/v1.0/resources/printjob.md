---
title: Tipo de recurso printJob
description: Representa um trabalho de impressão que foi ensuado para uma impressora.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d4c8d214c9a6cde11edc856f4682de1021486adf
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942510"
---
# <a name="printjob-resource-type"></a>Tipo de recurso printJob

Namespace: microsoft.graph

Representa um trabalho de impressão que foi ensuado para uma impressora.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/printjob-get.md) | [printJob](printjob.md) | Ler propriedades e relações do objeto printJob. |
| [Criar](../api/printer-post-jobs.md) | [printJob](printjob.md) | Crie um novo objeto de trabalho de impressão. |
| [Atualizar](../api/printjob-update.md) | [printJob](printjob.md) | Atualizar um objeto de trabalho de impressão. |
| [Start](../api/printjob-start.md)|Nenhum|Iniciar o trabalho de impressão.|
| [Cancel](../api/printjob-cancel.md)|Nenhum|Cancele o trabalho de impressão.|
| Anular**|Nenhum(a)|Aborte o trabalho de impressão.|
| [Redirecionar (para outra impressora)](../api/printjob-redirect.md) | [printJob](printjob.md) | Um trabalho de impressão que está na fila para a impressora de destino. |


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|GUID da impressora. Somente leitura.|
|createdDateTime|DateTimeOffset|DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|status|[printJobStatus](printjobstatus.md)|O status do trabalho de impressão. Somente leitura.|
|configuração|[printJobConfiguration](printJobConfiguration.md)|Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.|
|isFetchable|Edm.Boolean|Se true, o documento pode ser buscado pela impressora.|
|redirectedFrom|Edm.String|Contém a URL do trabalho de origem, se o trabalho tiver sido redirecionado de outra impressora.|
|redirectedTo|Edm.String|Contém a URL do trabalho de destino, se o trabalho tiver sido redirecionado para outra impressora.|
|createdBy|[userIdentity](useridentity.md)| Somente leitura. Anulável.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|documents|[Coleção printDocument](printdocument.md)| Somente leitura.|
|tarefas|[Coleção printTask](printtask.md)|Uma lista de [printTasks](printtask.md) que foram disparadas por esse trabalho de impressão.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printJob",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.printJobConfiguration"
  },
  "redirectedTo": "String",
  "redirectedFrom": "String",
  "isFetchable": "Boolean"
}
```

