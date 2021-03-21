---
title: Tipo de recurso directoryDefinition
description: Fornece informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8e3adb4679233fa35a53574b6f8d0c2b806be110
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956796"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="d2fd9-103">Tipo de recurso directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="d2fd9-103">directoryDefinition resource type</span></span>

<span data-ttu-id="d2fd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2fd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2fd9-105">Fornece informações do mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="d2fd9-106">Esse recurso informa ao mecanismo de sincronização, por exemplo, que o diretório tem objetos denominados **usuário** e grupo **,** quais atributos são suportados para esses objetos e os tipos para esses atributos.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="d2fd9-107">Para que o objeto e [](synchronization-synchronizationrule.md) o atributo participem de regras de sincronização e mapeamentos de objetos, eles devem ser [definidos](synchronization-objectmapping.md)como parte da definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="d2fd9-108">Em geral, o [esquema](synchronization-synchronizationschema.md) de sincronização [](synchronization-synchronizationtemplate.md) padrão fornecido como parte do modelo de sincronização definirá os objetos e atributos mais usados para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="d2fd9-109">No entanto, se o diretório suportar a adição de atributos personalizados, talvez você queira expandir a definição padrão com seus próprios objetos ou atributos personalizados.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="d2fd9-110">Para obter mais informações, consulte [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and Configure [synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="d2fd9-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="d2fd9-111">As definições de diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d2fd9-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d2fd9-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2fd9-112">Methods</span></span>

| <span data-ttu-id="d2fd9-113">Método</span><span class="sxs-lookup"><span data-stu-id="d2fd9-113">Method</span></span>       | <span data-ttu-id="d2fd9-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2fd9-114">Return Type</span></span>  |<span data-ttu-id="d2fd9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2fd9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2fd9-116">Descobrir directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="d2fd9-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="d2fd9-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="d2fd9-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="d2fd9-118">Descubra o esquema e as propriedades suportadas do diretório.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2fd9-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2fd9-119">Properties</span></span>

| <span data-ttu-id="d2fd9-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2fd9-120">Property</span></span>      | <span data-ttu-id="d2fd9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2fd9-121">Type</span></span>      | <span data-ttu-id="d2fd9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2fd9-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d2fd9-123">id</span><span class="sxs-lookup"><span data-stu-id="d2fd9-123">id</span></span>           |<span data-ttu-id="d2fd9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2fd9-124">String</span></span>     |<span data-ttu-id="d2fd9-125">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-125">Directory identifier.</span></span> <span data-ttu-id="d2fd9-126">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-126">Not nullable.</span></span>|
|<span data-ttu-id="d2fd9-127">metadados</span><span class="sxs-lookup"><span data-stu-id="d2fd9-127">metadata</span></span>       |<span data-ttu-id="d2fd9-128">Coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="d2fd9-128">metadataEntry collection</span></span>    |<span data-ttu-id="d2fd9-129">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-129">Additional extension properties.</span></span> <span data-ttu-id="d2fd9-130">A menos que mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="d2fd9-131">nome</span><span class="sxs-lookup"><span data-stu-id="d2fd9-131">name</span></span>           |<span data-ttu-id="d2fd9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2fd9-132">String</span></span>     |<span data-ttu-id="d2fd9-133">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-133">Name of the directory.</span></span> <span data-ttu-id="d2fd9-134">Deve ser exclusivo no esquema [de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d2fd9-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="d2fd9-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-135">Not nullable.</span></span>|
|<span data-ttu-id="d2fd9-136">objects</span><span class="sxs-lookup"><span data-stu-id="d2fd9-136">objects</span></span>        |<span data-ttu-id="d2fd9-137">[coleção objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2fd9-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="d2fd9-138">Coleção de objetos suportados pelo diretório.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="d2fd9-139">versão</span><span class="sxs-lookup"><span data-stu-id="d2fd9-139">version</span></span>|<span data-ttu-id="d2fd9-140">String</span><span class="sxs-lookup"><span data-stu-id="d2fd9-140">String</span></span>|<span data-ttu-id="d2fd9-141">Valor somente leitura que indica a versão descoberta.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="d2fd9-142">`null` se a descoberta ainda não tiver ocorrido.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-142">`null` if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="d2fd9-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="d2fd9-143">discoveryDateTime</span></span>|<span data-ttu-id="d2fd9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2fd9-144">DateTimeOffset</span></span>| <span data-ttu-id="d2fd9-145">Representa a data e a hora de descoberta usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d2fd9-146">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="d2fd9-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="d2fd9-147">discoverabilities</span></span>|<span data-ttu-id="d2fd9-148">directoryDefinitionDiscoverabilities</span><span class="sxs-lookup"><span data-stu-id="d2fd9-148">directoryDefinitionDiscoverabilities</span></span>| <span data-ttu-id="d2fd9-149">Valor somente leitura indicando que tipo de descoberta o aplicativo oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="d2fd9-150">Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="d2fd9-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2fd9-151">JSON representation</span></span>

<span data-ttu-id="d2fd9-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2fd9-152">The following is a JSON representation of the resource.</span></span>

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


