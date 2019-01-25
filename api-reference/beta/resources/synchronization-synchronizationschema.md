---
title: tipo de recurso de synchronizationSchema
description: Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica. Normalmente, você irá personalizar alguns dos mapeamentos de atributo ou adicionar um filtro de escopo para sincronizar apenas os objetos que atender a uma determinada condição.
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515927"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="1c229-105">tipo de recurso de synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1c229-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c229-106">Define quais objetos serão sincronizados e como eles serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="1c229-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="1c229-107">O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica.</span><span class="sxs-lookup"><span data-stu-id="1c229-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="1c229-108">Normalmente, você irá personalizar alguns dos [mapeamentos de atributo](synchronization-attributemapping.md)ou adicionar um [filtro de escopo](synchronization-filter.md) para sincronizar apenas os objetos que atender a uma determinada condição.</span><span class="sxs-lookup"><span data-stu-id="1c229-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="1c229-109">As seções a seguir descrevem os componentes de alto nível do esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1c229-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="1c229-110">Definições do diretório</span><span class="sxs-lookup"><span data-stu-id="1c229-110">Directory definitions</span></span>

<span data-ttu-id="1c229-111">[Definições de diretório](synchronization-directorydefinition.md) fornecem as informações de mecanismo de sincronização sobre diretórios e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="1c229-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="1c229-112">Por exemplo, a definição de diretório informa ao mecanismo de sincronização que um diretório do Windows Azure AD tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos.</span><span class="sxs-lookup"><span data-stu-id="1c229-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="1c229-113">Em ordem para um determinado objeto e o atributo a ser usado nos mapeamentos de objeto do rules de sincronização, eles devem ser definidos como parte da definição do diretório.</span><span class="sxs-lookup"><span data-stu-id="1c229-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="1c229-114">Regras de sincronização</span><span class="sxs-lookup"><span data-stu-id="1c229-114">Synchronization rules</span></span>

<span data-ttu-id="1c229-115">[Regras de sincronização](synchronization-synchronizationrule.md) são o núcleo da configuração da sincronização.</span><span class="sxs-lookup"><span data-stu-id="1c229-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="1c229-116">Elas definem para o mecanismo de sincronização como a sincronização deve ser executada, incluindo quais objetos devem ser sincronizados, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1c229-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="1c229-117">Mapeamentos de objeto</span><span class="sxs-lookup"><span data-stu-id="1c229-117">Object mappings</span></span>

<span data-ttu-id="1c229-118">[Mapeamentos de objeto](synchronization-objectmapping.md) são a parte principal da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1c229-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="1c229-119">Mapeamento de cada objeto define como um determinado objeto deve ser sincronizado da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1c229-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="1c229-120">Em particular, o mapeamento define como um objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, o que (se houver) filtros de escopo deve ser usado para decidir se deseja provisionar um objeto e como os atributos de objetos devem ser transformados Quando eles estão sincronizados da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1c229-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="1c229-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="1c229-121">Methods</span></span>

| <span data-ttu-id="1c229-122">Método</span><span class="sxs-lookup"><span data-stu-id="1c229-122">Method</span></span>        | <span data-ttu-id="1c229-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1c229-123">Return Type</span></span>               | <span data-ttu-id="1c229-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c229-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="1c229-125">Obter o esquema</span><span class="sxs-lookup"><span data-stu-id="1c229-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="1c229-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1c229-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="1c229-127">Leia as propriedades e os relacionamentos do objeto **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="1c229-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="1c229-128">Atualizar esquema</span><span class="sxs-lookup"><span data-stu-id="1c229-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="1c229-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c229-129">None</span></span>   |<span data-ttu-id="1c229-130">Atualize o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1c229-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="1c229-131">Excluir esquema</span><span class="sxs-lookup"><span data-stu-id="1c229-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="1c229-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c229-132">None</span></span>   |<span data-ttu-id="1c229-133">Exclua o esquema personalizado, redefinindo o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="1c229-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="1c229-134">Operadores de filtro de lista</span><span class="sxs-lookup"><span data-stu-id="1c229-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="1c229-135">coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)</span><span class="sxs-lookup"><span data-stu-id="1c229-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="1c229-136">Liste todos os operadores compatíveis com os filtros de escopo.</span><span class="sxs-lookup"><span data-stu-id="1c229-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="1c229-137">Funções de mapeamento de atributos de lista</span><span class="sxs-lookup"><span data-stu-id="1c229-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="1c229-138">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="1c229-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="1c229-139">Liste todas as funções que têm suportadas nas expressões de mapeamento do atributo.</span><span class="sxs-lookup"><span data-stu-id="1c229-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="1c229-140">Analisar expressão de mapeamento de atributo</span><span class="sxs-lookup"><span data-stu-id="1c229-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="1c229-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="1c229-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="1c229-142">Analisar uma expressão de cadeia de caracteres em uma [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="1c229-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="1c229-143">(.. / resources/synchronization_attributemappingsource.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="1c229-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="1c229-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c229-144">Properties</span></span>

| <span data-ttu-id="1c229-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c229-145">Property</span></span>      | <span data-ttu-id="1c229-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c229-146">Type</span></span>      | <span data-ttu-id="1c229-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c229-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1c229-148">diretórios</span><span class="sxs-lookup"><span data-stu-id="1c229-148">directories</span></span>            |<span data-ttu-id="1c229-149">coleção [directoryDefinition](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1c229-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="1c229-150">Descreve os objetos que fazem parte do [synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md)e diretórios.</span><span class="sxs-lookup"><span data-stu-id="1c229-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="1c229-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="1c229-151">synchronizationRules</span></span>   |<span data-ttu-id="1c229-152">coleção [synchronizationRule](synchronization-synchronizationrule.md)</span><span class="sxs-lookup"><span data-stu-id="1c229-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="1c229-153">Uma coleção de regras de sincronização configurados para o [synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span><span class="sxs-lookup"><span data-stu-id="1c229-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="1c229-154">version</span><span class="sxs-lookup"><span data-stu-id="1c229-154">version</span></span>                |<span data-ttu-id="1c229-155">String</span><span class="sxs-lookup"><span data-stu-id="1c229-155">String</span></span>                             |<span data-ttu-id="1c229-156">A versão do esquema, atualizado automaticamente com cada mudança de esquema.</span><span class="sxs-lookup"><span data-stu-id="1c229-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1c229-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c229-157">JSON representation</span></span>

<span data-ttu-id="1c229-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c229-158">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
