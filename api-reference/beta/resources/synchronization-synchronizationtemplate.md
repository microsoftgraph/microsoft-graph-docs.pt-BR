---
title: tipo de recurso synchronizationtemplate
description: " qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema de sincronização."
localization_priority: Normal
ms.openlocfilehash: fda63ede321de1a87604e7bca7fe7d7536d42689
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339851"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="fe1ee-103">tipo de recurso synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="fe1ee-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe1ee-104">Fornece configurações de sincronização pré-configuradas para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="fe1ee-105">Essas configurações serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) baseado no modelo.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="fe1ee-106">O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fe1ee-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="fe1ee-107">Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="fe1ee-108">Se vários modelos estiverem disponíveis para o aplicativo em que você está interessado, procure orientação específica do aplicativo para determinar qual deles atende melhor às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="fe1ee-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="fe1ee-109">Methods</span></span>

| <span data-ttu-id="fe1ee-110">Método</span><span class="sxs-lookup"><span data-stu-id="fe1ee-110">Method</span></span>        | <span data-ttu-id="fe1ee-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fe1ee-111">Return Type</span></span>               | <span data-ttu-id="fe1ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe1ee-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="fe1ee-113">List</span><span class="sxs-lookup"><span data-stu-id="fe1ee-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="fe1ee-114">[](synchronization-synchronizationtemplate.md) coleção synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="fe1ee-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="fe1ee-115">Lista os modelos disponíveis para uma instância de aplicativo ou aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="fe1ee-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="fe1ee-116">Get</span><span class="sxs-lookup"><span data-stu-id="fe1ee-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="fe1ee-117">synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="fe1ee-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="fe1ee-118">Leia as propriedades e as relações do \*\*\*\* objeto synchronizationtemplate.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="fe1ee-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe1ee-119">Properties</span></span>

| <span data-ttu-id="fe1ee-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe1ee-120">Property</span></span>      | <span data-ttu-id="fe1ee-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe1ee-121">Type</span></span>                      | <span data-ttu-id="fe1ee-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe1ee-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="fe1ee-123">id</span><span class="sxs-lookup"><span data-stu-id="fe1ee-123">id</span></span>             |<span data-ttu-id="fe1ee-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe1ee-124">String</span></span>                     |<span data-ttu-id="fe1ee-125">Identificador de modelo exclusivo.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-125">Unique template identifier.</span></span>|
|<span data-ttu-id="fe1ee-126">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="fe1ee-126">applicationId</span></span>  |<span data-ttu-id="fe1ee-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe1ee-127">String</span></span>                     |<span data-ttu-id="fe1ee-128">Identificador do aplicativo ao qual este modelo pertence.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="fe1ee-129">Padrão.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-129">default</span></span>        |<span data-ttu-id="fe1ee-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe1ee-130">Boolean</span></span>                    |<span data-ttu-id="fe1ee-131">`true`Se este modelo é recomendado para ser o padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="fe1ee-132">description</span><span class="sxs-lookup"><span data-stu-id="fe1ee-132">description</span></span>    |<span data-ttu-id="fe1ee-133">String</span><span class="sxs-lookup"><span data-stu-id="fe1ee-133">String</span></span>                     |<span data-ttu-id="fe1ee-134">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-134">Description of the template.</span></span>|
|<span data-ttu-id="fe1ee-135">detectáveis</span><span class="sxs-lookup"><span data-stu-id="fe1ee-135">discoverable</span></span>   |<span data-ttu-id="fe1ee-136">String</span><span class="sxs-lookup"><span data-stu-id="fe1ee-136">String</span></span>                     |<span data-ttu-id="fe1ee-137">`true`Se esse modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="fe1ee-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="fe1ee-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="fe1ee-138">factoryTag</span></span>     |<span data-ttu-id="fe1ee-139">String</span><span class="sxs-lookup"><span data-stu-id="fe1ee-139">String</span></span>                     |<span data-ttu-id="fe1ee-140">Uma das marcas de fábrica conhecidas suportadas pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="fe1ee-141">O **factoryTag** informa ao mecanismo de sincronização que implementação usar ao processar trabalhos com base nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="fe1ee-142">los</span><span class="sxs-lookup"><span data-stu-id="fe1ee-142">metadata</span></span>       |<span data-ttu-id="fe1ee-143">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="fe1ee-143">metadataEntry collection</span></span>   |<span data-ttu-id="fe1ee-144">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-144">Additional extension properties.</span></span> <span data-ttu-id="fe1ee-145">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe1ee-146">Relações</span><span class="sxs-lookup"><span data-stu-id="fe1ee-146">Relationships</span></span>
| <span data-ttu-id="fe1ee-147">Relação</span><span class="sxs-lookup"><span data-stu-id="fe1ee-147">Relationship</span></span>      | <span data-ttu-id="fe1ee-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe1ee-148">Type</span></span>      |<span data-ttu-id="fe1ee-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe1ee-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="fe1ee-150">esquemas</span><span class="sxs-lookup"><span data-stu-id="fe1ee-150">schema</span></span>             |[<span data-ttu-id="fe1ee-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="fe1ee-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="fe1ee-152">Esquema de sincronização padrão para os trabalhos baseados nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe1ee-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe1ee-153">JSON representation</span></span>

<span data-ttu-id="fe1ee-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe1ee-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
