---
title: Tipo de recurso groupPolicyUploadedDefinitionFile
description: A entidade representa um arquivo XML ADMX (Modelo Administrativo) carregado pelo Administrador. O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma DEPENDENTES ADML (Modelo Administrativo).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8f97a789fd7222aa585d339c4c74749455761b4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784783"
---
# <a name="grouppolicyuploadeddefinitionfile-resource-type"></a>Tipo de recurso groupPolicyUploadedDefinitionFile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um arquivo XML ADMX (Modelo Administrativo) carregado pelo Administrador. O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma DEPENDENTES ADML (Modelo Administrativo).


Herda de [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyUploadedDefinitionFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-list.md)|[coleção groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Listar propriedades e relações dos [objetos groupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|
|[Obter groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-get.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Leia propriedades e relações do [objeto groupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|
|[Criar groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-create.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Crie um novo [objeto groupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|
|[Excluir groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-delete.md)|Nenhum(a)|Exclui um [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md).|
|[Atualizar groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-update.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Atualize as propriedades de [um objeto groupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|
|[Ação addLanguageFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-addlanguagefiles.md)|Nenhuma|Ainda não documentado|
|[ação removeLanguageFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-removelanguagefiles.md)|Nenhuma|Ainda não documentado|
|[Ação updateLanguageFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-updatelanguagefiles.md)|Nenhuma|Ainda não documentado|
|[ação uploadNewVersion](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-uploadnewversion.md)|Nenhuma|Ainda não documentado|
|[remover ação](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-remove.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome amigável localizado do arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|descrição|Cadeia de caracteres|A descrição localizada das configurações de política no arquivo ADMX. O valor padrão é vazio. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|languageCodes|Coleção de cadeias de caracteres|Os códigos de idioma com suporte para o arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetPrefix|Cadeia de caracteres|Especifica o nome lógico que se refere ao namespace no arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetNamespace|Cadeia de caracteres|Especifica o URI usado para identificar o namespace no arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md). Os valores possíveis são: `admxBacked` e `admxIngested`.|
|revision|Cadeia de caracteres|A versão de revisão associada ao arquivo. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|O nome do arquivo ADML carregado.|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|O status de carregamento do arquivo ADMX carregado. Os valores possíveis são: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|conteúdo|Binário|O conteúdo do arquivo ADMX carregado.|
|uploadDateTime|DateTimeOffset|O tempo carregado do arquivo ADMX carregado.|
|defaultLanguageCode|Cadeia de caracteres|O idioma padrão do arquivo ADMX carregado.|
|groupPolicyUploadedLanguageFiles|[coleção groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)|A lista de arquivos ADML associados ao arquivo ADMX carregado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definições|[coleção groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|As definições de política de grupo associadas ao arquivo. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|groupPolicyOperations|[coleção groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|A lista de operações no arquivo ADMX carregado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "status": "String",
  "content": "binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "String",
      "languageCode": "String",
      "content": "binary",
      "id": "String",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```



