---
title: Tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (Modelo Administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma DEPENDENTES ADML (Modelo Administrativo).
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 884d2239eda3a86ed625fc2f7c1fa82e1bebd11a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086124"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>Tipo de recurso groupPolicyDefinitionFile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um arquivo XML ADMX (Modelo Administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma DEPENDENTES ADML (Modelo Administrativo).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Leia propriedades e relações do [objeto groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|[Atualizar groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Atualize as propriedades de [um objeto groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome amigável localizado do arquivo ADMX.|
|description|Cadeia de caracteres|A descrição localizada das configurações de política no arquivo ADMX. O valor padrão é vazio.|
|languageCodes|String collection|Os códigos de idioma com suporte para o arquivo ADMX.|
|targetPrefix|Cadeia de Caracteres|Especifica o nome lógico que se refere ao namespace no arquivo ADMX.|
|targetNamespace|Cadeia de Caracteres|Especifica o URI usado para identificar o namespace no arquivo ADMX.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Os valores possíveis são: `admxBacked` e `admxIngested`.|
|revision|Cadeia de Caracteres|A versão de revisão associada ao arquivo.|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definições|[coleção groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|As definições de política de grupo associadas ao arquivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
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
  "lastModifiedDateTime": "String (timestamp)"
}
```



