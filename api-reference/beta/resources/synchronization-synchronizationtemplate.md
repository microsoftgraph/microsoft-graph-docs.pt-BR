---
title: tipo de recurso synchronizationtemplate
description: Fornece configurações de sincronização pré-configuradas para um aplicativo específico.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d794391c4cf8043ab4eaeafcfa21958d93e3412a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985682"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="1e452-103">tipo de recurso synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="1e452-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="1e452-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e452-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e452-105">Fornece configurações de sincronização pré-configuradas para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="1e452-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="1e452-106">Essas configurações serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) baseado no modelo.</span><span class="sxs-lookup"><span data-stu-id="1e452-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="1e452-107">O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1e452-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="1e452-108">Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão.</span><span class="sxs-lookup"><span data-stu-id="1e452-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="1e452-109">Se vários modelos estiverem disponíveis para o aplicativo em que você está interessado, procure orientação específica do aplicativo para determinar qual deles atende melhor às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="1e452-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="1e452-110">Methods</span><span class="sxs-lookup"><span data-stu-id="1e452-110">Methods</span></span>

| <span data-ttu-id="1e452-111">Método</span><span class="sxs-lookup"><span data-stu-id="1e452-111">Method</span></span>        | <span data-ttu-id="1e452-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1e452-112">Return Type</span></span>               | <span data-ttu-id="1e452-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e452-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="1e452-114">List</span><span class="sxs-lookup"><span data-stu-id="1e452-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="1e452-115">coleção [synchronizationtemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1e452-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="1e452-116">Lista os modelos disponíveis para uma instância de aplicativo ou aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="1e452-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="1e452-117">Get</span><span class="sxs-lookup"><span data-stu-id="1e452-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="1e452-118">synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="1e452-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="1e452-119">Leia as propriedades e as relações do objeto **synchronizationtemplate** .</span><span class="sxs-lookup"><span data-stu-id="1e452-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="1e452-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e452-120">Properties</span></span>

| <span data-ttu-id="1e452-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e452-121">Property</span></span>      | <span data-ttu-id="1e452-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e452-122">Type</span></span>                      | <span data-ttu-id="1e452-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e452-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="1e452-124">id</span><span class="sxs-lookup"><span data-stu-id="1e452-124">id</span></span>             |<span data-ttu-id="1e452-125">String</span><span class="sxs-lookup"><span data-stu-id="1e452-125">String</span></span>                     |<span data-ttu-id="1e452-126">Identificador de modelo exclusivo.</span><span class="sxs-lookup"><span data-stu-id="1e452-126">Unique template identifier.</span></span>|
|<span data-ttu-id="1e452-127">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="1e452-127">applicationId</span></span>  |<span data-ttu-id="1e452-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e452-128">String</span></span>                     |<span data-ttu-id="1e452-129">Identificador do aplicativo ao qual este modelo pertence.</span><span class="sxs-lookup"><span data-stu-id="1e452-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="1e452-130">Padrão.</span><span class="sxs-lookup"><span data-stu-id="1e452-130">default</span></span>        |<span data-ttu-id="1e452-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e452-131">Boolean</span></span>                    |<span data-ttu-id="1e452-132">`true` Se este modelo é recomendado para ser o padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e452-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="1e452-133">description</span><span class="sxs-lookup"><span data-stu-id="1e452-133">description</span></span>    |<span data-ttu-id="1e452-134">String</span><span class="sxs-lookup"><span data-stu-id="1e452-134">String</span></span>                     |<span data-ttu-id="1e452-135">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="1e452-135">Description of the template.</span></span>|
|<span data-ttu-id="1e452-136">detectáveis</span><span class="sxs-lookup"><span data-stu-id="1e452-136">discoverable</span></span>   |<span data-ttu-id="1e452-137">String</span><span class="sxs-lookup"><span data-stu-id="1e452-137">String</span></span>                     |<span data-ttu-id="1e452-138">`true` Se esse modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="1e452-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="1e452-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="1e452-139">factoryTag</span></span>     |<span data-ttu-id="1e452-140">String</span><span class="sxs-lookup"><span data-stu-id="1e452-140">String</span></span>                     |<span data-ttu-id="1e452-141">Uma das marcas de fábrica conhecidas suportadas pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1e452-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="1e452-142">O **factoryTag** informa ao mecanismo de sincronização que implementação usar ao processar trabalhos com base nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="1e452-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="1e452-143">los</span><span class="sxs-lookup"><span data-stu-id="1e452-143">metadata</span></span>       |<span data-ttu-id="1e452-144">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="1e452-144">metadataEntry collection</span></span>   |<span data-ttu-id="1e452-145">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="1e452-145">Additional extension properties.</span></span> <span data-ttu-id="1e452-146">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="1e452-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e452-147">Relações</span><span class="sxs-lookup"><span data-stu-id="1e452-147">Relationships</span></span>
| <span data-ttu-id="1e452-148">Relação</span><span class="sxs-lookup"><span data-stu-id="1e452-148">Relationship</span></span>      | <span data-ttu-id="1e452-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e452-149">Type</span></span>      |<span data-ttu-id="1e452-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e452-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="1e452-151">esquemas</span><span class="sxs-lookup"><span data-stu-id="1e452-151">schema</span></span>             |[<span data-ttu-id="1e452-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1e452-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="1e452-153">Esquema de sincronização padrão para os trabalhos baseados nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="1e452-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e452-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e452-154">JSON representation</span></span>

<span data-ttu-id="1e452-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e452-155">The following is a JSON representation of the resource.</span></span>

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


