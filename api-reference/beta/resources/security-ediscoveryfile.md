---
title: Tipo de recurso ediscoveryFile
description: Representa um arquivo de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c47688daed5d5113c6b51fe096a06b93e78a8ae0
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837363"
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
|Extensão|String|A extensão de arquivo do arquivo, como png, msg, docx etc.|
|extractedTextContent|Stream|O texto extraído do arquivo original. Para arquivos baseados em imagem, esse seria o texto OCR.|
|id|Cadeia de caracteres|O identificador exclusivo do arquivo.|
|mediaType|String|mimeType do arquivo. Por exemplo: text/plain, charset=UTF-8, application/vnd.ms-outlook.|
|nome|String|O nome do arquivo. Assunto do email em caso de email.|
|otherProperties|microsoft.graph.security.stringValueDictionary|Uma lista de propriedades adicionais do arquivo, como titleOfSharepointDocument, emailRecipients. [Saiba mais](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).|
|processingStatus|microsoft.graph.security.fileProcessingStatus|O status de processamento depois que o item foi adicionado a um conjunto de revisão. Os valores possíveis são: , , , , , `invalidFileId`, , `fileSizeIsZero`, `fileDepthLimitExceeded``fileSizeIsTooLarge`, `fileBodyIsTooLong`, `fileTypeIsUnknown`, , `fileTypeIsNotSupported``malformedFile`, , `protectedFile`, `poisonFile`, , `noReviewSetSummaryGenerated`, `extractionException`, . `ocrProcessingTimeout``ocrFileSizeExceedsLimit``processingTimeout``unknownError``internalError``success`|
|senderAuthor|Coleção String|O remetente do email ou dos autores do documento.|
|size|Int64|tamanho do arquivo.|
|Sourcetype|microsoft.graph.security.sourceType|A origem original do conteúdo. Os valores possíveis são: `mailbox`, `site`.|
|subjectTitle|String|O assunto do email ou título do documento|

### <a name="fileprocessingstatus-values"></a>Valores fileProcessingStatus

|Member|Descrição|
|:----|-----------|
|sucesso|   O arquivo foi processado com êxito.|
|Internalerror| Exceção sem tratamento ocorreu durante o processamento do arquivo.|
|Unknownerror|o status do processamento é nulo ou vazio.|
|processingTimeout|O tempo limite ocorreu durante o processamento.|
|invalidFileId|Falha ao criar uma ID de campo exclusiva para o arquivo.|
|fileSizeIsZero|O tamanho do arquivo é zero ou negativo.|
|fileSizeIsTooLarge|O tamanho do arquivo excede os limites para processamento.|
|fileDepthLimitExceeded|A profundidade do arquivo excedeu o limite de processamento (30).|
|fileBodyIsTooLong|O comprimento dos textos no documento excede o limite de processamento.|
|fileTypeIsUnknown| Não há suporte para MimeType.|
|fileTypeIsNotSupported| Formato de arquivo sem suporte.|
|malformedFile|O arquivo está malformado.|
|protectedFile|Um email é protegido por direitos ou um documento é criptografado.|
|poisonFile|Arquivo já processado.|
|noReviewSetSummaryGenerated|Falha na geração do resumo do conjunto de revisão.|
|extractionException|Falha na extração de documentos inseridos.|
|ocrProcessingTimeout|Tempo limite durante o ocrProcessing do arquivo.|
|ocrFileSizeExceedsLimit|O tamanho do arquivo excede os limites para processamento de OCR.|


### <a name="datetime-values"></a>Valores de dateTime
|Tipo de arquivo|Definição|
|:---|:---|
Email |Data do envio.
Anexos de e-mail | Data da última modificação do documento; se não estiver disponível, a data de envio do pai.
Documentos incorporados | Data da última modificação do documento; se não estiver disponível, a data da última modificação do pai.
Documentos SPO (inclui anexos modernos) | Data da última modificação do SharePoint; se não estiver disponível, a data da última modificação dos documentos.
Documentos não Office 365 documentos | Data da última modificação.
Reuniões | Data de início da reunião.
Voicemail | Data do envio.
Mensagens instantâneas |Data do envio.
## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Custodiante|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Custodiantes associados ao arquivo.|
|tags|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Marcas associadas ao arquivo.|

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

