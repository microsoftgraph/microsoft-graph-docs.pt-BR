---
title: tipo de recurso de synchronizationTemplate
description: " qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema de sincronização."
ms.openlocfilehash: 90850ad43fdd14fc38ff6ae8cfa97f47806a289d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037230"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="c9796-103">tipo de recurso de synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="c9796-103">synchronizationTemplate resource type</span></span>

> <span data-ttu-id="c9796-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9796-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9796-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9796-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9796-106">Fornece configurações de sincronização pré-configurado para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9796-106">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="c9796-107">Essas configurações serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) que baseia-se no modelo.</span><span class="sxs-lookup"><span data-stu-id="c9796-107">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="c9796-108">O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c9796-108">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="c9796-109">Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão.</span><span class="sxs-lookup"><span data-stu-id="c9796-109">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="c9796-110">Se vários modelos estão disponíveis para o aplicativo que você está interessado, seek orientação específica de aplicativos para determinar qual deles melhor atenda às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="c9796-110">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="c9796-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9796-111">Methods</span></span>

| <span data-ttu-id="c9796-112">Método</span><span class="sxs-lookup"><span data-stu-id="c9796-112">Method</span></span>        | <span data-ttu-id="c9796-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9796-113">Return Type</span></span>               | <span data-ttu-id="c9796-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9796-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="c9796-115">List</span><span class="sxs-lookup"><span data-stu-id="c9796-115">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="c9796-116">coleção [synchronizationTemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c9796-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="c9796-117">Lista os modelos disponíveis para um aplicativo ou uma instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="c9796-117">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="c9796-118">Get</span><span class="sxs-lookup"><span data-stu-id="c9796-118">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="c9796-119">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="c9796-119">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="c9796-120">Leia as propriedades e relações do objeto **synchronizationTemplate** .</span><span class="sxs-lookup"><span data-stu-id="c9796-120">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="c9796-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9796-121">Properties</span></span>

| <span data-ttu-id="c9796-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9796-122">Property</span></span>      | <span data-ttu-id="c9796-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9796-123">Type</span></span>                      | <span data-ttu-id="c9796-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9796-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="c9796-125">id</span><span class="sxs-lookup"><span data-stu-id="c9796-125">id</span></span>             |<span data-ttu-id="c9796-126">String</span><span class="sxs-lookup"><span data-stu-id="c9796-126">String</span></span>                     |<span data-ttu-id="c9796-127">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="c9796-127">Unique template identifier.</span></span>|
|<span data-ttu-id="c9796-128">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="c9796-128">applicationId</span></span>  |<span data-ttu-id="c9796-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9796-129">String</span></span>                     |<span data-ttu-id="c9796-130">Identificador do aplicativo que pertence este modelo.</span><span class="sxs-lookup"><span data-stu-id="c9796-130">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="c9796-131">Padrão.</span><span class="sxs-lookup"><span data-stu-id="c9796-131">default</span></span>        |<span data-ttu-id="c9796-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="c9796-132">Boolean</span></span>                    |<span data-ttu-id="c9796-133">`true`Se esse modelo é recomendado para ser o padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9796-133">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="c9796-134">description</span><span class="sxs-lookup"><span data-stu-id="c9796-134">description</span></span>    |<span data-ttu-id="c9796-135">String</span><span class="sxs-lookup"><span data-stu-id="c9796-135">String</span></span>                     |<span data-ttu-id="c9796-136">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="c9796-136">Description of the template.</span></span>|
|<span data-ttu-id="c9796-137">detectáveis</span><span class="sxs-lookup"><span data-stu-id="c9796-137">discoverable</span></span>   |<span data-ttu-id="c9796-138">String</span><span class="sxs-lookup"><span data-stu-id="c9796-138">String</span></span>                     |<span data-ttu-id="c9796-139">`true`Se este modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="c9796-139">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="c9796-140">factoryTag</span><span class="sxs-lookup"><span data-stu-id="c9796-140">factoryTag</span></span>     |<span data-ttu-id="c9796-141">String</span><span class="sxs-lookup"><span data-stu-id="c9796-141">String</span></span>                     |<span data-ttu-id="c9796-142">Uma das marcas de fábrica conhecido suportadas pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c9796-142">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="c9796-143">O **factoryTag** informa ao mecanismo de sincronização qual implementação usar durante o processamento de trabalhos com base nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="c9796-143">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="c9796-144">metadados</span><span class="sxs-lookup"><span data-stu-id="c9796-144">metadata</span></span>       |<span data-ttu-id="c9796-145">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="c9796-145">metadataEntry collection</span></span>   |<span data-ttu-id="c9796-146">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="c9796-146">Additional extension properties.</span></span> <span data-ttu-id="c9796-147">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="c9796-147">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9796-148">Relações</span><span class="sxs-lookup"><span data-stu-id="c9796-148">Relationships</span></span>
| <span data-ttu-id="c9796-149">Relação</span><span class="sxs-lookup"><span data-stu-id="c9796-149">Relationship</span></span>      | <span data-ttu-id="c9796-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9796-150">Type</span></span>      |<span data-ttu-id="c9796-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9796-151">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="c9796-152">esquema</span><span class="sxs-lookup"><span data-stu-id="c9796-152">schema</span></span>             |[<span data-ttu-id="c9796-153">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c9796-153">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="c9796-154">Esquema de sincronização padrão para os trabalhos baseados nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="c9796-154">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9796-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9796-155">JSON representation</span></span>

<span data-ttu-id="c9796-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9796-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->