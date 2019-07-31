---
title: tipo de recurso synchronizationSchema
description: Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de configuração de um determinado trabalho de sincronização. Normalmente, você personalizará alguns dos mapeamentos de atributo ou adicionará um filtro de escopo para sincronizar somente objetos que atendam a uma determinada condição.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 95cb2a9bc38b3c23d8ddece5abe5520bf0fe25a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007778"
---
# <a name="synchronizationschema-resource-type"></a>tipo de recurso synchronizationSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de configuração de um determinado trabalho de sincronização. Normalmente, você personalizará alguns dos mapeamentos de [atributo](synchronization-attributemapping.md)ou adicionará um [filtro de escopo](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.

As seções a seguir descrevem os componentes de alto nível do esquema de sincronização.

## <a name="directory-definitions"></a>Definições de diretório

As [definições de diretório](synchronization-directorydefinition.md) fornecem as informações do mecanismo de sincronização sobre os diretórios e seus objetos. Por exemplo, a definição de diretório informa ao mecanismo de sincronização que um diretório do Azure AD possui objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos. Para que um determinado objeto e atributo seja usado em regras de sincronização/mapeamentos de objetos, eles precisam ser definidos como parte da definição de diretório.

## <a name="synchronization-rules"></a>Regras de sincronização

[As regras de sincronização](synchronization-synchronizationrule.md) são o núcleo da configuração de sincronização. Eles definem para o mecanismo de sincronização como a sincronização deve ser realizada, incluindo quais objetos devem ser sincronizados, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando estão sincronizados da origem para o diretório de destino. 

## <a name="object-mappings"></a>Mapeamentos de objetos

Os mapeamentos de [objeto](synchronization-objectmapping.md) são a parte principal da regra de sincronização. Cada mapeamento de objeto define como um determinado objeto deve ser sincronizado da origem para o diretório de destino. Em particular, o mapeamento define como um objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, quais filtros de escopo (se houver) devem ser usados para decidir se provisionar um objeto e como os atributos do objeto devem ser transformados Quando estão sincronizadas da origem para o diretório de destino.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[Obter esquema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Leia as propriedades e as relações do objeto **synchronizationSchema** .|
|[Atualizar esquema](../api/synchronization-synchronizationschema-update.md)    |Nenhum   |Atualize o esquema de sincronização. |
|[Excluir esquema](../api/synchronization-synchronizationschema-delete.md)    |Nenhum   |Exclua o esquema personalizado, redefinindo o esquema para a configuração padrão. |
|[Operadores de filtro de lista](../api/synchronization-synchronizationschema-filteroperators.md)    |coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)   |Liste todos os operadores com suporte nos filtros de escopo. |
|[Funções de mapeamento de atributo de lista](../api/synchronization-synchronizationschema-functions.md)    |coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)   |Listar todas as funções suportadas nas expressões de mapeamento de atributos. |
|[Analisar expressão de mapeamento de atributos](../api/synchronization-synchronizationschema-parseexpression.md)|[parseExpressionResponse](synchronization-parseexpressionresponse.md)|Analisar uma expressão de cadeia de caracteres em um [attributeMappingSource|(.. objeto/Resources/synchronization_attributemappingsource.MD).|


## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|diretórios            |coleção [directoryDefinition](synchronization-directorydefinition.md)   |Descreve os diretórios e os objetos que fazem parte do [synchronizationJob](synchronization-synchronizationjob.md) ou do [synchronizationtemplate](synchronization-synchronizationtemplate.md). |
|synchronizationRules   |coleção [synchronizationRule](synchronization-synchronizationrule.md)   |Uma coleção de regras de sincronização configuradas para o [synchronizationJob](synchronization-synchronizationjob.md) ou o [synchronizationtemplate](synchronization-synchronizationtemplate.md), |
|versão                |String                             |A versão do esquema, atualizada automaticamente com cada alteração de esquema.|


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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
