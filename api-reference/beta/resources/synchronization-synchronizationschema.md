---
title: tipo de recurso synchronizationSchema
description: Define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de configuração de um determinado trabalho de sincronização. Normalmente, você personalizará alguns dos mapeamentos de atributo ou adicionará um filtro de escopo para sincronizar somente objetos que atendam a uma determinada condição.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7d4302cec5fe568f322e5a8d1b86bc4681b50f7c
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620679"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="0813a-105">tipo de recurso synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0813a-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0813a-106">Define quais objetos serão sincronizados e como eles serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="0813a-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="0813a-107">O esquema de sincronização contém a maioria das informações de configuração de um determinado trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0813a-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="0813a-108">Normalmente, você personalizará alguns dos mapeamentos de [atributo](synchronization-attributemapping.md)ou adicionará um [filtro de escopo](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.</span><span class="sxs-lookup"><span data-stu-id="0813a-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="0813a-109">As seções a seguir descrevem os componentes de alto nível do esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0813a-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="0813a-110">Definições de diretório</span><span class="sxs-lookup"><span data-stu-id="0813a-110">Directory definitions</span></span>

<span data-ttu-id="0813a-111">As [definições de diretório](synchronization-directorydefinition.md) fornecem as informações do mecanismo de sincronização sobre os diretórios e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="0813a-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="0813a-112">Por exemplo, a definição de diretório informa ao mecanismo de sincronização que um diretório do Azure AD possui objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos.</span><span class="sxs-lookup"><span data-stu-id="0813a-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="0813a-113">Para que um determinado objeto e atributo seja usado em regras de sincronização/mapeamentos de objetos, eles precisam ser definidos como parte da definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="0813a-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="0813a-114">Regras de sincronização</span><span class="sxs-lookup"><span data-stu-id="0813a-114">Synchronization rules</span></span>

<span data-ttu-id="0813a-115">[As regras de sincronização](synchronization-synchronizationrule.md) são o núcleo da configuração de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0813a-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="0813a-116">Eles definem para o mecanismo de sincronização como a sincronização deve ser realizada, incluindo quais objetos devem ser sincronizados, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando estão sincronizados da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="0813a-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="0813a-117">Mapeamentos de objetos</span><span class="sxs-lookup"><span data-stu-id="0813a-117">Object mappings</span></span>

<span data-ttu-id="0813a-118">Os mapeamentos de [objeto](synchronization-objectmapping.md) são a parte principal da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0813a-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="0813a-119">Cada mapeamento de objeto define como um determinado objeto deve ser sincronizado da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="0813a-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="0813a-120">Em particular, o mapeamento define como um objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, quais filtros de escopo (se houver) devem ser usados para decidir se provisionar um objeto e como os atributos do objeto devem ser transformados Quando estão sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="0813a-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="0813a-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="0813a-121">Methods</span></span>

| <span data-ttu-id="0813a-122">Método</span><span class="sxs-lookup"><span data-stu-id="0813a-122">Method</span></span>        | <span data-ttu-id="0813a-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0813a-123">Return Type</span></span>               | <span data-ttu-id="0813a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0813a-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="0813a-125">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="0813a-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="0813a-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0813a-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="0813a-127">Leia as propriedades e as relações do objeto **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="0813a-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="0813a-128">Atualizar esquema</span><span class="sxs-lookup"><span data-stu-id="0813a-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="0813a-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0813a-129">None</span></span>   |<span data-ttu-id="0813a-130">Atualize o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0813a-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="0813a-131">Excluir esquema</span><span class="sxs-lookup"><span data-stu-id="0813a-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="0813a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0813a-132">None</span></span>   |<span data-ttu-id="0813a-133">Exclua o esquema personalizado, redefinindo o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="0813a-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="0813a-134">Operadores de filtro de lista</span><span class="sxs-lookup"><span data-stu-id="0813a-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="0813a-135">coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)</span><span class="sxs-lookup"><span data-stu-id="0813a-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="0813a-136">Liste todos os operadores com suporte nos filtros de escopo.</span><span class="sxs-lookup"><span data-stu-id="0813a-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="0813a-137">Funções de mapeamento de atributo de lista</span><span class="sxs-lookup"><span data-stu-id="0813a-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="0813a-138">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="0813a-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="0813a-139">Listar todas as funções suportadas nas expressões de mapeamento de atributos.</span><span class="sxs-lookup"><span data-stu-id="0813a-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="0813a-140">Analisar expressão de mapeamento de atributos</span><span class="sxs-lookup"><span data-stu-id="0813a-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="0813a-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="0813a-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="0813a-142">Analisar uma expressão de cadeia de caracteres em um [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="0813a-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="0813a-143">(.. objeto/Resources/synchronization_attributemappingsource.MD).</span><span class="sxs-lookup"><span data-stu-id="0813a-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="0813a-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0813a-144">Properties</span></span>

| <span data-ttu-id="0813a-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0813a-145">Property</span></span>      | <span data-ttu-id="0813a-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="0813a-146">Type</span></span>      | <span data-ttu-id="0813a-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="0813a-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0813a-148">diretórios</span><span class="sxs-lookup"><span data-stu-id="0813a-148">directories</span></span>            |<span data-ttu-id="0813a-149">coleção [directoryDefinition](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0813a-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="0813a-150">Descreve os diretórios e os objetos que fazem parte do [synchronizationJob](synchronization-synchronizationjob.md) ou do [synchronizationtemplate](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0813a-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="0813a-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="0813a-151">synchronizationRules</span></span>   |<span data-ttu-id="0813a-152">coleção [synchronizationRule](synchronization-synchronizationrule.md)</span><span class="sxs-lookup"><span data-stu-id="0813a-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="0813a-153">Uma coleção de regras de sincronização configuradas para o [synchronizationJob](synchronization-synchronizationjob.md) ou o [synchronizationtemplate](synchronization-synchronizationtemplate.md),</span><span class="sxs-lookup"><span data-stu-id="0813a-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="0813a-154">versão</span><span class="sxs-lookup"><span data-stu-id="0813a-154">version</span></span>                |<span data-ttu-id="0813a-155">String</span><span class="sxs-lookup"><span data-stu-id="0813a-155">String</span></span>                             |<span data-ttu-id="0813a-156">A versão do esquema, atualizada automaticamente com cada alteração de esquema.</span><span class="sxs-lookup"><span data-stu-id="0813a-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0813a-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0813a-157">JSON representation</span></span>

<span data-ttu-id="0813a-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0813a-158">The following is a JSON representation of the resource.</span></span>

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
