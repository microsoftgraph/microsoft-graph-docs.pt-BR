---
title: Tipo de recurso groupPolicyUploadedLanguageFile
description: A entidade representa um arquivo XML ADML (idioma do modelo administrativo) carregado pelo Administrador.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c25c35c32c1c127cf00c9d0d7e968177450b1065
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046768"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>Tipo de recurso groupPolicyUploadedLanguageFile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um arquivo XML ADML (idioma do modelo administrativo) carregado pelo Administrador.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|fileName|String|O nome do arquivo ADML carregado.|
|languageCode|Cadeia de Caracteres|O código de idioma do arquivo ADML carregado.|
|conteúdo|Binário|O conteúdo do arquivo ADML carregado.|
|id|Cadeia de caracteres|Chave da entidade.|
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



