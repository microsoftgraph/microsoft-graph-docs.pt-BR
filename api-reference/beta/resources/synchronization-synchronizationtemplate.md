---
title: tipo de recurso de synchronizationTemplate
description: " qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema de sincronização."
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516550"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="2067b-103">tipo de recurso de synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="2067b-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2067b-104">Fornece configurações de sincronização pré-configurado para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2067b-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="2067b-105">Essas configurações serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) que baseia-se no modelo.</span><span class="sxs-lookup"><span data-stu-id="2067b-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="2067b-106">O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2067b-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="2067b-107">Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão.</span><span class="sxs-lookup"><span data-stu-id="2067b-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="2067b-108">Se vários modelos estão disponíveis para o aplicativo que você está interessado, seek orientação específica de aplicativos para determinar qual deles melhor atenda às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="2067b-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="2067b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2067b-109">Methods</span></span>

| <span data-ttu-id="2067b-110">Método</span><span class="sxs-lookup"><span data-stu-id="2067b-110">Method</span></span>        | <span data-ttu-id="2067b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2067b-111">Return Type</span></span>               | <span data-ttu-id="2067b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2067b-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="2067b-113">List</span><span class="sxs-lookup"><span data-stu-id="2067b-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="2067b-114">coleção [synchronizationTemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="2067b-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="2067b-115">Lista os modelos disponíveis para um aplicativo ou uma instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="2067b-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="2067b-116">Get</span><span class="sxs-lookup"><span data-stu-id="2067b-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="2067b-117">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="2067b-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="2067b-118">Leia as propriedades e relações do objeto **synchronizationTemplate** .</span><span class="sxs-lookup"><span data-stu-id="2067b-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="2067b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2067b-119">Properties</span></span>

| <span data-ttu-id="2067b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2067b-120">Property</span></span>      | <span data-ttu-id="2067b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2067b-121">Type</span></span>                      | <span data-ttu-id="2067b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2067b-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="2067b-123">id</span><span class="sxs-lookup"><span data-stu-id="2067b-123">id</span></span>             |<span data-ttu-id="2067b-124">String</span><span class="sxs-lookup"><span data-stu-id="2067b-124">String</span></span>                     |<span data-ttu-id="2067b-125">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="2067b-125">Unique template identifier.</span></span>|
|<span data-ttu-id="2067b-126">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="2067b-126">applicationId</span></span>  |<span data-ttu-id="2067b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2067b-127">String</span></span>                     |<span data-ttu-id="2067b-128">Identificador do aplicativo que pertence este modelo.</span><span class="sxs-lookup"><span data-stu-id="2067b-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="2067b-129">Padrão.</span><span class="sxs-lookup"><span data-stu-id="2067b-129">default</span></span>        |<span data-ttu-id="2067b-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="2067b-130">Boolean</span></span>                    |<span data-ttu-id="2067b-131">`true`Se esse modelo é recomendado para ser o padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2067b-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="2067b-132">description</span><span class="sxs-lookup"><span data-stu-id="2067b-132">description</span></span>    |<span data-ttu-id="2067b-133">String</span><span class="sxs-lookup"><span data-stu-id="2067b-133">String</span></span>                     |<span data-ttu-id="2067b-134">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="2067b-134">Description of the template.</span></span>|
|<span data-ttu-id="2067b-135">detectáveis</span><span class="sxs-lookup"><span data-stu-id="2067b-135">discoverable</span></span>   |<span data-ttu-id="2067b-136">String</span><span class="sxs-lookup"><span data-stu-id="2067b-136">String</span></span>                     |<span data-ttu-id="2067b-137">`true`Se este modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="2067b-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="2067b-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="2067b-138">factoryTag</span></span>     |<span data-ttu-id="2067b-139">String</span><span class="sxs-lookup"><span data-stu-id="2067b-139">String</span></span>                     |<span data-ttu-id="2067b-140">Uma das marcas de fábrica conhecido suportadas pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2067b-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="2067b-141">O **factoryTag** informa ao mecanismo de sincronização qual implementação usar durante o processamento de trabalhos com base nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="2067b-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="2067b-142">Metadata</span><span class="sxs-lookup"><span data-stu-id="2067b-142">metadata</span></span>       |<span data-ttu-id="2067b-143">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="2067b-143">metadataEntry collection</span></span>   |<span data-ttu-id="2067b-144">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="2067b-144">Additional extension properties.</span></span> <span data-ttu-id="2067b-145">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="2067b-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2067b-146">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="2067b-146">Relationships</span></span>
| <span data-ttu-id="2067b-147">Relação</span><span class="sxs-lookup"><span data-stu-id="2067b-147">Relationship</span></span>      | <span data-ttu-id="2067b-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="2067b-148">Type</span></span>      |<span data-ttu-id="2067b-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="2067b-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="2067b-150">SCHEMA</span><span class="sxs-lookup"><span data-stu-id="2067b-150">schema</span></span>             |[<span data-ttu-id="2067b-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="2067b-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="2067b-152">Esquema de sincronização padrão para os trabalhos baseados nesse modelo.</span><span class="sxs-lookup"><span data-stu-id="2067b-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2067b-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2067b-153">JSON representation</span></span>

<span data-ttu-id="2067b-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2067b-154">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
