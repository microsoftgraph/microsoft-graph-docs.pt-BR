---
title: Tipo de recurso synchronizationTemplate
description: Fornece configurações de sincronização pré-configuradas para um aplicativo específico.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c08f5c3eee6225a1149ff993415f83b2e5916583
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132297"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="96638-103">Tipo de recurso synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="96638-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="96638-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96638-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96638-105">Fornece configurações de sincronização pré-configuradas para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96638-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="96638-106">Essas configurações serão usadas por padrão para qualquer trabalho [de](synchronization-synchronizationjob.md) sincronização baseado no modelo.</span><span class="sxs-lookup"><span data-stu-id="96638-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="96638-107">O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema [de sincronização.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="96638-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="96638-108">Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão.</span><span class="sxs-lookup"><span data-stu-id="96638-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="96638-109">Se vários modelos estão disponíveis para o aplicativo em que você está interessado, procure orientações específicas do aplicativo para determinar qual deles atende melhor às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="96638-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="96638-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="96638-110">Methods</span></span>

| <span data-ttu-id="96638-111">Método</span><span class="sxs-lookup"><span data-stu-id="96638-111">Method</span></span>        | <span data-ttu-id="96638-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96638-112">Return Type</span></span>               | <span data-ttu-id="96638-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="96638-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="96638-114">List</span><span class="sxs-lookup"><span data-stu-id="96638-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="96638-115">[Coleção synchronizationTemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="96638-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="96638-116">Liste os modelos que estão disponíveis para uma instância de aplicativo ou aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="96638-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="96638-117">Get</span><span class="sxs-lookup"><span data-stu-id="96638-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="96638-118">synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="96638-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="96638-119">Leia as propriedades e os relacionamentos do **objeto synchronizationTemplate.**</span><span class="sxs-lookup"><span data-stu-id="96638-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="96638-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96638-120">Properties</span></span>

| <span data-ttu-id="96638-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96638-121">Property</span></span>      | <span data-ttu-id="96638-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="96638-122">Type</span></span>                      | <span data-ttu-id="96638-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="96638-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="96638-124">id</span><span class="sxs-lookup"><span data-stu-id="96638-124">id</span></span>             |<span data-ttu-id="96638-125">String</span><span class="sxs-lookup"><span data-stu-id="96638-125">String</span></span>                     |<span data-ttu-id="96638-126">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="96638-126">Unique template identifier.</span></span>|
|<span data-ttu-id="96638-127">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="96638-127">applicationId</span></span>  |<span data-ttu-id="96638-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96638-128">String</span></span>                     |<span data-ttu-id="96638-129">Identificador do aplicativo ao que este modelo pertence.</span><span class="sxs-lookup"><span data-stu-id="96638-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="96638-130">Padrão.</span><span class="sxs-lookup"><span data-stu-id="96638-130">default</span></span>        |<span data-ttu-id="96638-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="96638-131">Boolean</span></span>                    |<span data-ttu-id="96638-132">`true` se esse modelo for recomendado para ser o padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96638-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="96638-133">description</span><span class="sxs-lookup"><span data-stu-id="96638-133">description</span></span>    |<span data-ttu-id="96638-134">String</span><span class="sxs-lookup"><span data-stu-id="96638-134">String</span></span>                     |<span data-ttu-id="96638-135">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="96638-135">Description of the template.</span></span>|
|<span data-ttu-id="96638-136">discoverable</span><span class="sxs-lookup"><span data-stu-id="96638-136">discoverable</span></span>   |<span data-ttu-id="96638-137">String</span><span class="sxs-lookup"><span data-stu-id="96638-137">String</span></span>                     |<span data-ttu-id="96638-138">`true` se esse modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="96638-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="96638-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="96638-139">factoryTag</span></span>     |<span data-ttu-id="96638-140">String</span><span class="sxs-lookup"><span data-stu-id="96638-140">String</span></span>                     |<span data-ttu-id="96638-141">Uma das marcas de fábrica conhecidas com suporte no mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="96638-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="96638-142">A **factoryTag** informa ao mecanismo de sincronização qual implementação usar ao processar trabalhos baseados nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="96638-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="96638-143">metadados</span><span class="sxs-lookup"><span data-stu-id="96638-143">metadata</span></span>       |<span data-ttu-id="96638-144">Coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="96638-144">metadataEntry collection</span></span>   |<span data-ttu-id="96638-145">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="96638-145">Additional extension properties.</span></span> <span data-ttu-id="96638-146">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="96638-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96638-147">Relações</span><span class="sxs-lookup"><span data-stu-id="96638-147">Relationships</span></span>
| <span data-ttu-id="96638-148">Relação</span><span class="sxs-lookup"><span data-stu-id="96638-148">Relationship</span></span>      | <span data-ttu-id="96638-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="96638-149">Type</span></span>      |<span data-ttu-id="96638-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="96638-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="96638-151">schema</span><span class="sxs-lookup"><span data-stu-id="96638-151">schema</span></span>             |[<span data-ttu-id="96638-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="96638-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="96638-153">Esquema de sincronização padrão para os trabalhos baseados neste modelo.</span><span class="sxs-lookup"><span data-stu-id="96638-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96638-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96638-154">JSON representation</span></span>

<span data-ttu-id="96638-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96638-155">The following is a JSON representation of the resource.</span></span>

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


