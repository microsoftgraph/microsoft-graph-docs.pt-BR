---
title: Tipo de recurso ediscoveryFile
description: Representa um arquivo de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6e952dcc8299b43817fca48beb4a705c522d12f4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945048"
---
# <a name="ediscoveryfile-resource-type"></a>Tipo de recurso ediscoveryFile

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade que representa arquivos ReviewSet de descoberta eletrônica.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryFiles](../api/security-ediscoveryreviewset-list-files.md)|[coleção microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Obtenha uma lista dos [objetos ediscoveryFile](../resources/security-ediscoveryfile.md) e suas propriedades.|
|[Obter ediscoveryFile](../api/security-ediscoveryfile-get.md)|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Leia as propriedades e as relações de [um objeto ediscoveryFile](../resources/security-ediscoveryfile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conteúdo|Fluxo|O fluxo de conteúdo do arquivo original.|
|dateTime|DateTimeOffset|O datetime em que o arquivo foi modificado pela última vez. Consulte os valores de dateTime para obter mais detalhes.|
|Extensão|Cadeia de caracteres|A extensão de arquivo do arquivo, como png, msg, docx etc.|
|extractedTextContent|Fluxo|O texto extraído do arquivo original. Para arquivos baseados em imagem, esse seria o texto OCR.|
|id|String|O identificador exclusivo do arquivo.|
|mediaType|Cadeia de caracteres|mimeType do arquivo. Por exemplo: text/plain, charset=UTF-8, application/vnd.ms-outlook.|
|nome|Cadeia de caracteres|O nome do arquivo. Assunto do email em caso de email.|
|otherProperties|Cadeia de caracteres|Uma lista de propriedades adicionais do arquivo, como titleOfSharepointDocument, emailRecipients. [Saiba mais](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).|
|processingStatus|String|O status de processamento depois que o item foi adicionado a um conjunto de revisão. Os valores possíveis são: , , , , , `invalidFileId`, , `fileSizeIsZero`, `fileDepthLimitExceeded``fileSizeIsTooLarge`, `fileBodyIsTooLong`, `fileTypeIsUnknown`, , `fileTypeIsNotSupported``malformedFile`, , `protectedFile`, `poisonFile`, , `noReviewSetSummaryGenerated`, `extractionException`, . `ocrProcessingTimeout``ocrFileSizeExceedsLimit``processingTimeout``unknownError``internalError``success`|
|senderAuthor|Coleção de cadeias de caracteres|O remetente do email ou dos autores do documento.|
|size|Int64|tamanho do arquivo.|
|Sourcetype|Cadeia de caracteres|A origem original do conteúdo. Os valores possíveis são: `mailbox`, `site`.|
|subjectTitle|Cadeia de caracteres|O assunto do email ou título do documento|

### <a name="datetime-values"></a>Valores de dateTime
|Tipo de arquivo|Definição|
|:---|:---|
Email |Data do envio.
Anexos de e-mail | Data da última modificação do documento; se não estiver disponível, a data de envio do pai.
Documentos incorporados | Data da última modificação do documento; se não estiver disponível, a data da última modificação do pai.
Documentos SPO (inclui anexos modernos) | Data da última modificação do SharePoint; se não estiver disponível, a data da última modificação dos documentos.
Documentos que não são do Office 365 | Data da última modificação.
Reuniões | Data de início da reunião.
Voicemail | Data do envio.
Mensagens instantâneas |Data do envio.
## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Custodiante|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Custodiantes associados ao arquivo.|
|categorias|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Marcas associadas ao arquivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryFile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryFile",
  "id": "String (identifier)",
  "dateTime": "String (timestamp)",
  "size": "Integer",
  "name": "String",
  "sourceType": "String",
  "senderAuthor": [
    "String"
  ],
  "subjectTitle": "String",
  "extension": "String",
  "mediaType": "String",
  "content": "Stream",
  "extractedTextContent": "Stream",
  "processingStatus": "String",
  "otherProperties": {
    "@odata.type": "microsoft.graph.security.stringValueDictionary"
  }
}
```

