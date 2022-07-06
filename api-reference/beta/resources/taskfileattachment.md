---
title: Tipo de recurso taskFileAttachment
description: Representa um arquivo, como um arquivo de texto ou documento do Word, anexado a um todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1724222d362edae4f053af58ce52680052a15be7
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645602"
---
# <a name="taskfileattachment-resource-type"></a>Tipo de recurso taskFileAttachment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um arquivo, como um arquivo de texto ou documento do Word, anexado a um [todoTask](../resources/todotask.md).
Quando você cria um anexo de arquivo em uma tarefa, inclua `"@odata.type": "#microsoft.graph.taskFileAttachment"` e o nome das **propriedades e** **contentBytes**.

Herda de [attachmentBase](../resources/attachmentbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar anexos](../api/todotask-list-attachments.md)|[Coleção taskFileAttachment](../resources/taskfileattachment.md)|Obtenha uma lista dos [objetos taskFileAttachment](../resources/taskfileattachment.md) e suas propriedades.|
|[Criar anexo](../api/todotask-post-attachments.md)|[Coleção taskFileAttachment](../resources/taskfileattachment.md)|Adicione um novo [objeto taskFileAttachment](../resources/taskfileattachment.md) a um [todoTask](../resources/todotask.md).|
|[Criar sessão de upload](../api/taskfileattachment-createuploadsession.md)|[Coleção taskFileAttachment](../resources/taskfileattachment.md)|Crie uma sessão de upload para carregar iterativamente intervalos de um arquivo como um anexo para um [todoTask](../resources/todotask.md).|
|[Obter anexo](../api/taskfileattachment-get.md)|[taskFileAttachment](../resources/taskfileattachment.md)|Leia as propriedades e as relações de um [objeto taskFileAttachment](../resources/taskfileattachment.md) .|
|[Excluir anexo](../api/taskfileattachment-delete.md)|Nenhum|[Exclua um objeto taskFileAttachment](../resources/taskfileattachment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentBytes|Binária|O conteúdo do arquivo codificado pela base64.|
|contentType|String|O tipo de conteúdo do anexo. Herdado do [attachmentBase](../resources/attachmentbase.md).|
|id|Cadeia de caracteres|A ID do anexo. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez. Herdado do [attachmentBase](../resources/attachmentbase.md).|
|nome|Cadeia de caracteres|O nome do texto exibido sob o ícone que representa o anexo inserido. Não precisa ser o nome real do arquivo. Herdado do [attachmentBase](../resources/attachmentbase.md).|
|size|Int32|O tamanho do anexo em bytes. Herdado do [attachmentBase](../resources/attachmentbase.md).|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taskFileAttachment",
  "baseType": "microsoft.graph.attachmentBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "contentBytes": "Binary",
  "contentType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": "Int32"
}
```

