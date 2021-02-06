---
title: Tipo de recurso synchronizationSchema
description: Define quais objetos serão sincronizados e como eles serão sincronizados.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b16e892c44cb69fb5039418a4a246e8b6f32ae9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131590"
---
# <a name="synchronizationschema-resource-type"></a>Tipo de recurso synchronizationSchema

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de configuração para um trabalho de sincronização específico. Normalmente, você personalizará alguns dos [mapeamentos](synchronization-attributemapping.md)de atributos ou adicionará um filtro de [scoping](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.

As seções a seguir descrevem os componentes de alto nível do esquema de sincronização.

## <a name="directory-definitions"></a>Definições de diretório

[As definições de diretório](synchronization-directorydefinition.md) fornecem as informações do mecanismo de sincronização sobre diretórios e seus objetos. Por exemplo, a definição de diretório informa ao mecanismo de  sincronização que um diretório do Azure AD tem objetos chamados usuário e **grupo,** quais atributos são suportados para esses objetos e os tipos para esses atributos. Para que um determinado objeto e atributo seja usado em mapeamentos de regras/objetos de sincronização, eles precisam ser definidos como parte da definição de diretório.

## <a name="synchronization-rules"></a>Regras de sincronização

[As regras de sincronização](synchronization-synchronizationrule.md) são o núcleo da configuração de sincronização. Eles definem para o mecanismo de sincronização como a sincronização deve ser executada, incluindo quais objetos devem ser sincronizados, como os objetos do diretório de origem devem ser corresponder aos objetos no diretório de destino e como os atributos devem ser transformados quando são sincronizados da origem para o diretório de destino.

## <a name="object-mappings"></a>Mapeamentos de objetos

[Mapeamentos de objetos](synchronization-objectmapping.md) são a parte principal da regra de sincronização. Cada mapeamento de objeto define como um determinado objeto deve ser sincronizado da origem para o diretório de destino. Em particular, o mapeamento define como um objeto no diretório de origem deve ser parecido com um objeto no diretório de destino, quais filtros de scoping (se algum) devem ser usados para decidir se provisionar um objeto e como os atributos de objeto devem ser transformados quando são sincronizados da origem para o diretório de destino.

## <a name="methods"></a>Métodos

| Método                                                                                                | Tipo de retorno                                                                                                 | Descrição                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [Obter esquema](../api/synchronization-synchronizationschema-get.md)                                     | [synchronizationSchema](synchronization-synchronizationschema.md)                                           | Leia as propriedades e as relações do **objeto synchronizationSchema.**                                                 |
| [Atualizar esquema](../api/synchronization-synchronizationschema-update.md)                               | Nenhuma                                                                                                        | Atualize o esquema de sincronização.                                                                                         |
| [Excluir esquema](../api/synchronization-synchronizationschema-delete.md)                               | Nenhuma                                                                                                        | Exclua o esquema personalizado, redefinindo o esquema para a configuração padrão.                                           |
| [Listar operadores de filtro](../api/synchronization-synchronizationschema-filteroperators.md)              | [Coleção filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)                      | Lista todos os operadores com suporte nos filtros de seleção.                                                                       |
| [Listar funções de mapeamento de atributos](../api/synchronization-synchronizationschema-functions.md)         | [Coleção attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) | Lista todas as funções com suporte nas expressões de mapeamento de atributos.                                                         |
| [Expressão de mapeamento de atributo de análise](../api/synchronization-synchronizationschema-parseexpression.md) | [parseExpressionResponse](synchronization-parseexpressionresponse.md)                                       | Analisar uma expressão de cadeia de caracteres em [um objeto attributeMappingSource.](../resources/synchronization-attributemappingsource.md) |


## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id|String|Identificador exclusivo do esquema.|
|synchronizationRules   |[Coleção synchronizationRule](synchronization-synchronizationrule.md)   |Uma coleção de regras de sincronização configuradas para [o synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md). |
|versão                |String                             |A versão do esquema, atualizada automaticamente a cada alteração de esquema.|


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|directories|[Coleção directoryDefinition](../resources/synchronization-directorydefinition.md)|Contém a coleção de diretórios e todos os seus objetos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "String (identifier)",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```


