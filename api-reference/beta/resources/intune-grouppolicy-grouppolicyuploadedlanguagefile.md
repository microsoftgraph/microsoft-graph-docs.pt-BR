---
title: tipo de recurso groupPolicyUploadedLanguageFile
description: A entidade representa um arquivo XML de ADML (idioma de modelo administrativo) carregado pelo administrador.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc70d0ff85cebc567b9efc67b87bb57e2e8337fa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707686"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>tipo de recurso groupPolicyUploadedLanguageFile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um arquivo XML de ADML (idioma de modelo administrativo) carregado pelo administrador.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|fileName|String|O nome de arquivo do arquivo ADML carregado.|
|Campo|String|O código de idioma do arquivo ADML carregado.|
|conteúdo|Binária|O conteúdo do arquivo ADML carregado.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedLanguageFile",
  "fileName": "String",
  "languageCode": "String",
  "content": "binary",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





