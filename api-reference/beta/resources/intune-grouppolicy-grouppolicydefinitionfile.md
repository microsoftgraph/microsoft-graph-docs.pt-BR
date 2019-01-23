---
title: tipo de recurso de groupPolicyDefinitionFile
description: A entidade representa um arquivo XML de ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus respectivos locais pelo caminho de categoria. O arquivo de definição de diretiva de grupo também contém os idiomas com suporte conforme determinado pelos arquivos de idioma ADML (Administrative Template) dependentes de idioma.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431261"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>tipo de recurso de groupPolicyDefinitionFile

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A entidade representa um arquivo XML de ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus respectivos locais pelo caminho de categoria. O arquivo de definição de diretiva de grupo também contém os idiomas com suporte conforme determinado pelos arquivos de idioma ADML (Administrative Template) dependentes de idioma.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|
|[Atualizar groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Atualize as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome amigável localizado do arquivo ADMX.|
|description|String|A descrição localizada das configurações de política no arquivo ADMX. O valor padrão é vazio.|
|languageCodes|String collection|Os códigos de idioma com suporte para o arquivo ADMX.|
|targetPrefix|String|Especifica o nome lógico que se refere ao namespace no arquivo ADMX.|
|targetNamespace|String|Especifica o URI usado para identificar o namespace no arquivo ADMX.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Os valores possíveis são: `admxBacked` e `admxIngested`.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definições|coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|As definições de política de grupo associadas ao arquivo.|

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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




