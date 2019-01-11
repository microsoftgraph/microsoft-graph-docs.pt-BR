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
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="e429d-105">tipo de recurso de synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e429d-105">synchronizationSchema resource type</span></span>

> <span data-ttu-id="e429d-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e429d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e429d-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e429d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e429d-108">Define quais objetos serão sincronizados e como eles serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="e429d-108">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="e429d-109">O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica.</span><span class="sxs-lookup"><span data-stu-id="e429d-109">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="e429d-110">Normalmente, você irá personalizar alguns dos [mapeamentos de atributo](synchronization-attributemapping.md)ou adicionar um [filtro de escopo](synchronization-filter.md) para sincronizar apenas os objetos que atender a uma determinada condição.</span><span class="sxs-lookup"><span data-stu-id="e429d-110">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="e429d-111">As seções a seguir descrevem os componentes de alto nível do esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e429d-111">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="e429d-112">Definições do diretório</span><span class="sxs-lookup"><span data-stu-id="e429d-112">Directory definitions</span></span>

<span data-ttu-id="e429d-113">[Definições de diretório](synchronization-directorydefinition.md) fornecem as informações de mecanismo de sincronização sobre diretórios e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="e429d-113">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="e429d-114">Por exemplo, a definição de diretório informa ao mecanismo de sincronização que um diretório do Windows Azure AD tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos.</span><span class="sxs-lookup"><span data-stu-id="e429d-114">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="e429d-115">Em ordem para um determinado objeto e o atributo a ser usado nos mapeamentos de objeto do rules de sincronização, eles devem ser definidos como parte da definição do diretório.</span><span class="sxs-lookup"><span data-stu-id="e429d-115">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="e429d-116">Regras de sincronização</span><span class="sxs-lookup"><span data-stu-id="e429d-116">Synchronization rules</span></span>

<span data-ttu-id="e429d-117">[Regras de sincronização](synchronization-synchronizationrule.md) são o núcleo da configuração da sincronização.</span><span class="sxs-lookup"><span data-stu-id="e429d-117">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="e429d-118">Elas definem para o mecanismo de sincronização como a sincronização deve ser executada, incluindo quais objetos devem ser sincronizados, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="e429d-118">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="e429d-119">Mapeamentos de objeto</span><span class="sxs-lookup"><span data-stu-id="e429d-119">Object mappings</span></span>

<span data-ttu-id="e429d-120">[Mapeamentos de objeto](synchronization-objectmapping.md) são a parte principal da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e429d-120">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="e429d-121">Mapeamento de cada objeto define como um determinado objeto deve ser sincronizado da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="e429d-121">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="e429d-122">Em particular, o mapeamento define como um objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, o que (se houver) filtros de escopo deve ser usado para decidir se deseja provisionar um objeto e como os atributos de objetos devem ser transformados Quando eles estão sincronizados da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="e429d-122">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="e429d-123">Métodos</span><span class="sxs-lookup"><span data-stu-id="e429d-123">Methods</span></span>

| <span data-ttu-id="e429d-124">Método</span><span class="sxs-lookup"><span data-stu-id="e429d-124">Method</span></span>        | <span data-ttu-id="e429d-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e429d-125">Return Type</span></span>               | <span data-ttu-id="e429d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e429d-126">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="e429d-127">Obter o esquema</span><span class="sxs-lookup"><span data-stu-id="e429d-127">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="e429d-128">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e429d-128">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="e429d-129">Leia as propriedades e os relacionamentos do objeto **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="e429d-129">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="e429d-130">Atualizar esquema</span><span class="sxs-lookup"><span data-stu-id="e429d-130">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="e429d-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e429d-131">None</span></span>   |<span data-ttu-id="e429d-132">Atualize o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e429d-132">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="e429d-133">Excluir esquema</span><span class="sxs-lookup"><span data-stu-id="e429d-133">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="e429d-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e429d-134">None</span></span>   |<span data-ttu-id="e429d-135">Exclua o esquema personalizado, redefinindo o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="e429d-135">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="e429d-136">Operadores de filtro de lista</span><span class="sxs-lookup"><span data-stu-id="e429d-136">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="e429d-137">coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)</span><span class="sxs-lookup"><span data-stu-id="e429d-137">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="e429d-138">Liste todos os operadores compatíveis com os filtros de escopo.</span><span class="sxs-lookup"><span data-stu-id="e429d-138">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="e429d-139">Funções de mapeamento de atributos de lista</span><span class="sxs-lookup"><span data-stu-id="e429d-139">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="e429d-140">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="e429d-140">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="e429d-141">Liste todas as funções que têm suportadas nas expressões de mapeamento do atributo.</span><span class="sxs-lookup"><span data-stu-id="e429d-141">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="e429d-142">Analisar expressão de mapeamento de atributo</span><span class="sxs-lookup"><span data-stu-id="e429d-142">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="e429d-143">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="e429d-143">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="e429d-144">Analisar uma expressão de cadeia de caracteres em uma [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e429d-144">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="e429d-145">(.. / resources/synchronization_attributemappingsource.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="e429d-145">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="e429d-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e429d-146">Properties</span></span>

| <span data-ttu-id="e429d-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e429d-147">Property</span></span>      | <span data-ttu-id="e429d-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="e429d-148">Type</span></span>      | <span data-ttu-id="e429d-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="e429d-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e429d-150">diretórios</span><span class="sxs-lookup"><span data-stu-id="e429d-150">directories</span></span>            |<span data-ttu-id="e429d-151">coleção [directoryDefinition](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e429d-151">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="e429d-152">Descreve os objetos que fazem parte do [synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md)e diretórios.</span><span class="sxs-lookup"><span data-stu-id="e429d-152">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="e429d-153">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="e429d-153">synchronizationRules</span></span>   |<span data-ttu-id="e429d-154">coleção [synchronizationRule](synchronization-synchronizationrule.md)</span><span class="sxs-lookup"><span data-stu-id="e429d-154">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="e429d-155">Uma coleção de regras de sincronização configurados para o [synchronizationJob](synchronization-synchronizationjob.md) ou [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span><span class="sxs-lookup"><span data-stu-id="e429d-155">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="e429d-156">version</span><span class="sxs-lookup"><span data-stu-id="e429d-156">version</span></span>                |<span data-ttu-id="e429d-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e429d-157">String</span></span>                             |<span data-ttu-id="e429d-158">A versão do esquema, atualizado automaticamente com cada mudança de esquema.</span><span class="sxs-lookup"><span data-stu-id="e429d-158">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e429d-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e429d-159">JSON representation</span></span>

<span data-ttu-id="e429d-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e429d-160">The following is a JSON representation of the resource.</span></span>

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
