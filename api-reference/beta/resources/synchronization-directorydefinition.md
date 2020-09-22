---
title: tipo de recurso directoryDefinition
description: Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ccafa9d6763339c32102ace1572c85148f793fc6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089284"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="c0ae1-103">tipo de recurso directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="c0ae1-103">directoryDefinition resource type</span></span>

<span data-ttu-id="c0ae1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0ae1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0ae1-105">Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="c0ae1-106">Esse recurso instrui o mecanismo de sincronização, por exemplo, que o diretório tem objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="c0ae1-107">Para que o objeto e o atributo participem das [regras de sincronização](synchronization-synchronizationrule.md) e dos [mapeamentos de objetos](synchronization-objectmapping.md), eles devem ser definidos como parte da definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="c0ae1-108">Em geral, o [esquema de sincronização](synchronization-synchronizationschema.md) padrão fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá os objetos e atributos usados com mais frequência para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="c0ae1-109">No entanto, se o diretório oferecer suporte à adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos ou atributos personalizados.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="c0ae1-110">Para obter mais informações, consulte [Configurar a sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e [Configurar a sincronização com atributos de extensão de diretório](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="c0ae1-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="c0ae1-111">As definições de diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c0ae1-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c0ae1-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0ae1-112">Methods</span></span>

| <span data-ttu-id="c0ae1-113">Método</span><span class="sxs-lookup"><span data-stu-id="c0ae1-113">Method</span></span>       | <span data-ttu-id="c0ae1-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0ae1-114">Return Type</span></span>  |<span data-ttu-id="c0ae1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0ae1-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0ae1-116">Descobrir directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="c0ae1-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="c0ae1-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="c0ae1-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="c0ae1-118">Descubra o esquema e as propriedades com suporte do diretório.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0ae1-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0ae1-119">Properties</span></span>

| <span data-ttu-id="c0ae1-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0ae1-120">Property</span></span>      | <span data-ttu-id="c0ae1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0ae1-121">Type</span></span>      | <span data-ttu-id="c0ae1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0ae1-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c0ae1-123">id</span><span class="sxs-lookup"><span data-stu-id="c0ae1-123">id</span></span>           |<span data-ttu-id="c0ae1-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0ae1-124">String</span></span>     |<span data-ttu-id="c0ae1-125">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-125">Directory identifier.</span></span> <span data-ttu-id="c0ae1-126">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-126">Not nullable.</span></span>|
|<span data-ttu-id="c0ae1-127">los</span><span class="sxs-lookup"><span data-stu-id="c0ae1-127">metadata</span></span>       |<span data-ttu-id="c0ae1-128">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="c0ae1-128">metadataEntry collection</span></span>    |<span data-ttu-id="c0ae1-129">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-129">Additional extension properties.</span></span> <span data-ttu-id="c0ae1-130">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c0ae1-131">name</span><span class="sxs-lookup"><span data-stu-id="c0ae1-131">name</span></span>           |<span data-ttu-id="c0ae1-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0ae1-132">String</span></span>     |<span data-ttu-id="c0ae1-133">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-133">Name of the directory.</span></span> <span data-ttu-id="c0ae1-134">Deve ser exclusivo no [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c0ae1-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="c0ae1-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-135">Not nullable.</span></span>|
|<span data-ttu-id="c0ae1-136">objectos</span><span class="sxs-lookup"><span data-stu-id="c0ae1-136">objects</span></span>        |<span data-ttu-id="c0ae1-137">coleção [ObjectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0ae1-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="c0ae1-138">Conjunto de objetos suportados pelo diretório.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="c0ae1-139">versão</span><span class="sxs-lookup"><span data-stu-id="c0ae1-139">version</span></span>|<span data-ttu-id="c0ae1-140">String</span><span class="sxs-lookup"><span data-stu-id="c0ae1-140">String</span></span>|<span data-ttu-id="c0ae1-141">Valor somente leitura que indica a versão descoberta.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="c0ae1-142">NULL se a descoberta ainda não tiver ocorrido.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-142">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="c0ae1-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ae1-143">discoveryDateTime</span></span>|<span data-ttu-id="c0ae1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ae1-144">DateTimeOffset</span></span>| <span data-ttu-id="c0ae1-145">Representa a data e a hora da descoberta usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c0ae1-146">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c0ae1-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c0ae1-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="c0ae1-147">discoverabilities</span></span>|<span data-ttu-id="c0ae1-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0ae1-148">string</span></span>| <span data-ttu-id="c0ae1-149">Valor somente leitura indicando qual tipo de descoberta o aplicativo oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="c0ae1-150">Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="c0ae1-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0ae1-151">JSON representation</span></span>

<span data-ttu-id="c0ae1-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0ae1-152">The following is a JSON representation of the resource.</span></span>

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


