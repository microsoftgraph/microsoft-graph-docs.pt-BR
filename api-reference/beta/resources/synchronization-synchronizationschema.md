---
title: tipo de recurso de synchronizationSchema
description: Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica. Normalmente, você irá personalizar alguns dos mapeamentos de atributo ou adicionar um filtro de escopo para sincronizar apenas os objetos que atender a uma determinada condição.
localization_priority: Normal
ms.openlocfilehash: 696bdbbc6fa2d96965d11a12fb09fdfc0ce16106
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847317"
---
# <a name="synchronizationschema-resource-type"></a>tipo de recurso de synchronizationSchema

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica. Normalmente, você irá personalizar alguns dos [mapeamentos de atributo](synchronization-attributemapping.md)ou adicionar um [filtro de escopo](synchronization-filter.md) para sincronizar apenas os objetos que atender a uma determinada condição.

As seções a seguir descrevem os componentes de alto nível do esquema de sincronização.

## <a name="directory-definitions"></a>Definições do diretório

[Definições de diretório](synchronization-directorydefinition.md) fornecem as informações de mecanismo de sincronização sobre diretórios e seus objetos. Por exemplo, a definição de diretório informa ao mecanismo de sincronização que um diretório do Windows Azure AD tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos. Em ordem para um determinado objeto e o atributo a ser usado nos mapeamentos de objeto do rules de sincronização, eles devem ser definidos como parte da definição do diretório.

## <a name="synchronization-rules"></a>Regras de sincronização

[Regras de sincronização](synchronization-synchronizationrule.md) são o núcleo da configuração da sincronização. Elas definem para o mecanismo de sincronização como a sincronização deve ser executada, incluindo quais objetos devem ser sincronizados, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando elas estiver sincronizadas da origem para o diretório de destino. 

## <a name="object-mappings"></a>Mapeamentos de objeto

[Mapeamentos de objeto](synchronization-objectmapping.md) são a parte principal da regra de sincronização. Mapeamento de cada objeto define como um determinado objeto deve ser sincronizado da origem para o diretório de destino. Em particular, o mapeamento define como um objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, o que (se houver) filtros de escopo deve ser usado para decidir se deseja provisionar um objeto e como os atributos de objetos devem ser transformados Quando eles estão sincronizados da origem para o diretório de destino.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[Obter o esquema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Leia as propriedades e os relacionamentos do objeto **synchronizationSchema** .|
|[Atualizar esquema](../api/synchronization-synchronizationschema-update.md)    |Nenhum   |Atualize o esquema de sincronização. |
|[Excluir esquema](../api/synchronization-synchronizationschema-delete.md)    |Nenhum   |Exclua o esquema personalizado, redefinindo o esquema para a configuração padrão. |
|[Operadores de filtro de lista](../api/synchronization-synchronizationschema-filteroperators.md)    |coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)   |Liste todos os operadores compatíveis com os filtros de escopo. |
|[Funções de mapeamento de atributos de lista](../api/synchronization-synchronizationschema-functions.md)    |coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)   |Liste todas as funções que têm suportadas nas expressões de mapeamento do atributo. |
|[Analisar expressão de mapeamento de atributo](../api/synchronization-synchronizationschema-parseexpression.md)|[parseExpressionResponse](synchronization-parseexpressionresponse.md)|Analisar uma expressão de cadeia de caracteres em uma [attributeMappingSource|(.. / resources/synchronization_attributemappingsource.md) objeto.|


## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|diretórios            |coleção [directoryDefinition](synchronization-directorydefinition.md)   |Descreve os objetos que fazem parte do [synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md)e diretórios. |
|synchronizationRules   |coleção [synchronizationRule](synchronization-synchronizationrule.md)   |Uma coleção de regras de sincronização configurados para o [synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md), |
|version                |Cadeia de caracteres                             |A versão do esquema, atualizado automaticamente com cada mudança de esquema.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
