---
title: tipo de recurso directoryDefinition
description: Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56c1f5a6a15f7ab6724feff68aa38eba1ef22694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888136"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="b09e4-103">tipo de recurso directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="b09e4-103">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b09e4-104">Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="b09e4-104">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="b09e4-105">Esse recurso instrui o mecanismo de sincronização, por exemplo, que o diretório tem objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos.</span><span class="sxs-lookup"><span data-stu-id="b09e4-105">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="b09e4-106">Para que o objeto e o atributo participem das [regras de sincronização](synchronization-synchronizationrule.md) e dos mapeamentos de [objetos](synchronization-objectmapping.md), eles devem ser definidos como parte da definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="b09e4-106">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="b09e4-107">Em geral, o [esquema de sincronização](synchronization-synchronizationschema.md) padrão fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá os objetos e atributos usados com mais frequência para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="b09e4-107">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="b09e4-108">No entanto, se o diretório oferecer suporte à adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos ou atributos personalizados.</span><span class="sxs-lookup"><span data-stu-id="b09e4-108">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="b09e4-109">Para obter mais informações, consulte [Configurar a sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e [Configurar a sincronização com atributos de extensão de diretório](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="b09e4-109">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="b09e4-110">As definições de diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="b09e4-110">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b09e4-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="b09e4-111">Methods</span></span>

| <span data-ttu-id="b09e4-112">Método</span><span class="sxs-lookup"><span data-stu-id="b09e4-112">Method</span></span>       | <span data-ttu-id="b09e4-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b09e4-113">Return Type</span></span>  |<span data-ttu-id="b09e4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b09e4-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b09e4-115">Descobrir directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="b09e4-115">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="b09e4-116">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="b09e4-116">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="b09e4-117">Descubra o esquema e as propriedades com suporte do diretório.</span><span class="sxs-lookup"><span data-stu-id="b09e4-117">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="b09e4-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b09e4-118">Properties</span></span>

| <span data-ttu-id="b09e4-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b09e4-119">Property</span></span>      | <span data-ttu-id="b09e4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b09e4-120">Type</span></span>      | <span data-ttu-id="b09e4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b09e4-121">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="b09e4-122">id</span><span class="sxs-lookup"><span data-stu-id="b09e4-122">id</span></span>           |<span data-ttu-id="b09e4-123">String</span><span class="sxs-lookup"><span data-stu-id="b09e4-123">String</span></span>     |<span data-ttu-id="b09e4-124">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="b09e4-124">Directory identifier.</span></span> <span data-ttu-id="b09e4-125">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="b09e4-125">Not nullable.</span></span>|
|<span data-ttu-id="b09e4-126">los</span><span class="sxs-lookup"><span data-stu-id="b09e4-126">metadata</span></span>       |<span data-ttu-id="b09e4-127">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="b09e4-127">metadataEntry collection</span></span>    |<span data-ttu-id="b09e4-128">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="b09e4-128">Additional extension properties.</span></span> <span data-ttu-id="b09e4-129">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="b09e4-129">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="b09e4-130">name</span><span class="sxs-lookup"><span data-stu-id="b09e4-130">name</span></span>           |<span data-ttu-id="b09e4-131">String</span><span class="sxs-lookup"><span data-stu-id="b09e4-131">String</span></span>     |<span data-ttu-id="b09e4-132">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="b09e4-132">Name of the directory.</span></span> <span data-ttu-id="b09e4-133">Deve ser exclusivo no [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="b09e4-133">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="b09e4-134">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="b09e4-134">Not nullable.</span></span>|
|<span data-ttu-id="b09e4-135">objectos</span><span class="sxs-lookup"><span data-stu-id="b09e4-135">objects</span></span>        |<span data-ttu-id="b09e4-136">[](synchronization-objectdefinition.md) coleção ObjectDefinition</span><span class="sxs-lookup"><span data-stu-id="b09e4-136">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="b09e4-137">Conjunto de objetos suportados pelo diretório.</span><span class="sxs-lookup"><span data-stu-id="b09e4-137">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="b09e4-138">versão</span><span class="sxs-lookup"><span data-stu-id="b09e4-138">version</span></span>|<span data-ttu-id="b09e4-139">String</span><span class="sxs-lookup"><span data-stu-id="b09e4-139">String</span></span>|<span data-ttu-id="b09e4-140">Valor somente leitura que indica a versão descoberta.</span><span class="sxs-lookup"><span data-stu-id="b09e4-140">Read only value that indicates version discovered.</span></span> <span data-ttu-id="b09e4-141">NULL se a descoberta ainda não tiver ocorrido.</span><span class="sxs-lookup"><span data-stu-id="b09e4-141">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="b09e4-142">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="b09e4-142">discoveryDateTime</span></span>|<span data-ttu-id="b09e4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b09e4-143">DateTimeOffset</span></span>| <span data-ttu-id="b09e4-144">Representa a data e a hora da descoberta usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b09e4-144">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b09e4-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b09e4-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b09e4-146">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="b09e4-146">discoverabilities</span></span>|<span data-ttu-id="b09e4-147">string</span><span class="sxs-lookup"><span data-stu-id="b09e4-147">string</span></span>| <span data-ttu-id="b09e4-148">Valor somente leitura indicando qual tipo de descoberta o aplicativo oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="b09e4-148">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="b09e4-149">Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b09e4-149">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="b09e4-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b09e4-150">JSON representation</span></span>

<span data-ttu-id="b09e4-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b09e4-151">The following is a JSON representation of the resource.</span></span>

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
