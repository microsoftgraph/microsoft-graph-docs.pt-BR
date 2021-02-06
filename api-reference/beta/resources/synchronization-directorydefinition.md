---
title: Tipo de recurso directoryDefinition
description: Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 77af192ff09cf557eec3e73c1973c4c71dc39a96
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134047"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="e29f5-103">Tipo de recurso directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e29f5-103">directoryDefinition resource type</span></span>

<span data-ttu-id="e29f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e29f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e29f5-105">Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="e29f5-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="e29f5-106">Esse recurso informa ao mecanismo de sincronização, por  exemplo, que o diretório tem objetos chamados usuário e **grupo,** quais atributos são suportados para esses objetos e os tipos para esses atributos.</span><span class="sxs-lookup"><span data-stu-id="e29f5-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="e29f5-107">Para que o objeto e [](synchronization-synchronizationrule.md) o atributo participem de regras de sincronização e mapeamentos de objetos, eles devem ser [definidos](synchronization-objectmapping.md)como parte da definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="e29f5-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="e29f5-108">Em geral, o [esquema](synchronization-synchronizationschema.md) de sincronização [](synchronization-synchronizationtemplate.md) padrão fornecido como parte do modelo de sincronização definirá os objetos e atributos mais usados para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="e29f5-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="e29f5-109">No entanto, se o diretório suportar a adição de atributos personalizados, talvez você queira expandir a definição padrão com seus próprios objetos ou atributos personalizados.</span><span class="sxs-lookup"><span data-stu-id="e29f5-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="e29f5-110">Para obter mais informações, [consulte Configurar a sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e [configurar a sincronização com atributos de extensão de diretório.](synchronization-configure-with-directory-extension-attributes.md)</span><span class="sxs-lookup"><span data-stu-id="e29f5-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="e29f5-111">As definições de diretório são atualizadas como parte [do esquema de sincronização.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="e29f5-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e29f5-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="e29f5-112">Methods</span></span>

| <span data-ttu-id="e29f5-113">Método</span><span class="sxs-lookup"><span data-stu-id="e29f5-113">Method</span></span>       | <span data-ttu-id="e29f5-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e29f5-114">Return Type</span></span>  |<span data-ttu-id="e29f5-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e29f5-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e29f5-116">Descobrir directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e29f5-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="e29f5-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e29f5-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="e29f5-118">Descubra o esquema e as propriedades com suporte do diretório.</span><span class="sxs-lookup"><span data-stu-id="e29f5-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="e29f5-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e29f5-119">Properties</span></span>

| <span data-ttu-id="e29f5-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e29f5-120">Property</span></span>      | <span data-ttu-id="e29f5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e29f5-121">Type</span></span>      | <span data-ttu-id="e29f5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e29f5-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e29f5-123">id</span><span class="sxs-lookup"><span data-stu-id="e29f5-123">id</span></span>           |<span data-ttu-id="e29f5-124">String</span><span class="sxs-lookup"><span data-stu-id="e29f5-124">String</span></span>     |<span data-ttu-id="e29f5-125">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="e29f5-125">Directory identifier.</span></span> <span data-ttu-id="e29f5-126">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e29f5-126">Not nullable.</span></span>|
|<span data-ttu-id="e29f5-127">metadados</span><span class="sxs-lookup"><span data-stu-id="e29f5-127">metadata</span></span>       |<span data-ttu-id="e29f5-128">Coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="e29f5-128">metadataEntry collection</span></span>    |<span data-ttu-id="e29f5-129">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="e29f5-129">Additional extension properties.</span></span> <span data-ttu-id="e29f5-130">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="e29f5-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="e29f5-131">nome</span><span class="sxs-lookup"><span data-stu-id="e29f5-131">name</span></span>           |<span data-ttu-id="e29f5-132">String</span><span class="sxs-lookup"><span data-stu-id="e29f5-132">String</span></span>     |<span data-ttu-id="e29f5-133">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="e29f5-133">Name of the directory.</span></span> <span data-ttu-id="e29f5-134">Deve ser exclusivo no esquema [de sincronização.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="e29f5-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="e29f5-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e29f5-135">Not nullable.</span></span>|
|<span data-ttu-id="e29f5-136">objects</span><span class="sxs-lookup"><span data-stu-id="e29f5-136">objects</span></span>        |<span data-ttu-id="e29f5-137">[coleção objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e29f5-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="e29f5-138">Coleção de objetos com suporte no diretório.</span><span class="sxs-lookup"><span data-stu-id="e29f5-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="e29f5-139">versão</span><span class="sxs-lookup"><span data-stu-id="e29f5-139">version</span></span>|<span data-ttu-id="e29f5-140">String</span><span class="sxs-lookup"><span data-stu-id="e29f5-140">String</span></span>|<span data-ttu-id="e29f5-141">Valor somente leitura que indica a versão descoberta.</span><span class="sxs-lookup"><span data-stu-id="e29f5-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="e29f5-142">Nulo se a descoberta ainda não tiver ocorrido.</span><span class="sxs-lookup"><span data-stu-id="e29f5-142">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="e29f5-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="e29f5-143">discoveryDateTime</span></span>|<span data-ttu-id="e29f5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e29f5-144">DateTimeOffset</span></span>| <span data-ttu-id="e29f5-145">Representa a data e a hora de descoberta usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e29f5-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e29f5-146">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e29f5-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e29f5-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="e29f5-147">discoverabilities</span></span>|<span data-ttu-id="e29f5-148">string</span><span class="sxs-lookup"><span data-stu-id="e29f5-148">string</span></span>| <span data-ttu-id="e29f5-149">Valor somente leitura indicando que tipo de descoberta o aplicativo oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="e29f5-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="e29f5-150">Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e29f5-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="e29f5-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e29f5-151">JSON representation</span></span>

<span data-ttu-id="e29f5-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e29f5-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


