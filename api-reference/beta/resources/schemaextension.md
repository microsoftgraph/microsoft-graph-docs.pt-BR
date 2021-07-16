---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 43e5600ea7e8fb8a484216e8068c9ac3f29ac90d
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456398"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="2d04f-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="2d04f-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="2d04f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d04f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d04f-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="2d04f-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="2d04f-108">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="2d04f-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="2d04f-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2d04f-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="2d04f-110">contact</span><span class="sxs-lookup"><span data-stu-id="2d04f-110">contact</span></span>](contact.md)
- [<span data-ttu-id="2d04f-111">device</span><span class="sxs-lookup"><span data-stu-id="2d04f-111">device</span></span>](device.md)
- <span data-ttu-id="2d04f-112">[event](event.md) em um usuário ou calendário de grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2d04f-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="2d04f-113">[post](post.md) de um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2d04f-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="2d04f-114">grupo</span><span class="sxs-lookup"><span data-stu-id="2d04f-114">group</span></span>](group.md)
- [<span data-ttu-id="2d04f-115">message</span><span class="sxs-lookup"><span data-stu-id="2d04f-115">message</span></span>](message.md) 
- [<span data-ttu-id="2d04f-116">organization</span><span class="sxs-lookup"><span data-stu-id="2d04f-116">organization</span></span>](organization.md)
- [<span data-ttu-id="2d04f-117">user</span><span class="sxs-lookup"><span data-stu-id="2d04f-117">user</span></span>](user.md)

<span data-ttu-id="2d04f-118">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="2d04f-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="2d04f-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="2d04f-119">Methods</span></span>

| <span data-ttu-id="2d04f-120">Método</span><span class="sxs-lookup"><span data-stu-id="2d04f-120">Method</span></span>           | <span data-ttu-id="2d04f-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d04f-121">Return Type</span></span>    |<span data-ttu-id="2d04f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d04f-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d04f-123">Criar</span><span class="sxs-lookup"><span data-stu-id="2d04f-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="2d04f-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="2d04f-124">schemaExtension</span></span> |<span data-ttu-id="2d04f-125">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="2d04f-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="2d04f-126">Listar</span><span class="sxs-lookup"><span data-stu-id="2d04f-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="2d04f-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="2d04f-127">schemaExtension</span></span> |<span data-ttu-id="2d04f-128">Listar as definições do esquema de avaialbeExtension e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2d04f-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="2d04f-129">Get</span><span class="sxs-lookup"><span data-stu-id="2d04f-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="2d04f-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="2d04f-130">schemaExtension</span></span> |<span data-ttu-id="2d04f-131">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="2d04f-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="2d04f-132">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2d04f-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="2d04f-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="2d04f-133">schemaExtension</span></span>   |<span data-ttu-id="2d04f-134">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="2d04f-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="2d04f-135">Excluir</span><span class="sxs-lookup"><span data-stu-id="2d04f-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="2d04f-136">None</span><span class="sxs-lookup"><span data-stu-id="2d04f-136">None</span></span> |<span data-ttu-id="2d04f-137">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="2d04f-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d04f-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d04f-138">Properties</span></span>
| <span data-ttu-id="2d04f-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d04f-139">Property</span></span>     | <span data-ttu-id="2d04f-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d04f-140">Type</span></span>   |<span data-ttu-id="2d04f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d04f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d04f-142">description</span><span class="sxs-lookup"><span data-stu-id="2d04f-142">description</span></span>|<span data-ttu-id="2d04f-143">String</span><span class="sxs-lookup"><span data-stu-id="2d04f-143">String</span></span>|<span data-ttu-id="2d04f-144">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="2d04f-144">Description for the schema extension.</span></span> <span data-ttu-id="2d04f-145">Suporta `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="2d04f-145">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="2d04f-146">id</span><span class="sxs-lookup"><span data-stu-id="2d04f-146">id</span></span>|<span data-ttu-id="2d04f-147">String</span><span class="sxs-lookup"><span data-stu-id="2d04f-147">String</span></span>|<span data-ttu-id="2d04f-148">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="2d04f-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="2d04f-149">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="2d04f-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="2d04f-p104">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="2d04f-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="2d04f-p105">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="2d04f-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="2d04f-154">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="2d04f-154">This property cannot be changed after creation.</span></span> <span data-ttu-id="2d04f-155">Suporta `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="2d04f-155">Supports `$filter` (`eq`).</span></span> |
|<span data-ttu-id="2d04f-156">proprietário</span><span class="sxs-lookup"><span data-stu-id="2d04f-156">owner</span></span>|<span data-ttu-id="2d04f-157">String</span><span class="sxs-lookup"><span data-stu-id="2d04f-157">String</span></span>| <span data-ttu-id="2d04f-158">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="2d04f-158">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="2d04f-159">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="2d04f-159">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="2d04f-160">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="2d04f-160">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="2d04f-161">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d04f-161">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="2d04f-162">Então, por exemplo, se criar uma nova definição de extensão do esquema usando o Explorador do Graph, você **deverá** fornecer a propriedade de proprietário.</span><span class="sxs-lookup"><span data-stu-id="2d04f-162">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="2d04f-163">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="2d04f-163">Once set, this property is read-only and cannot be changed.</span></span> <span data-ttu-id="2d04f-164">Suporta `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="2d04f-164">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="2d04f-165">properties</span><span class="sxs-lookup"><span data-stu-id="2d04f-165">properties</span></span>|<span data-ttu-id="2d04f-166">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2d04f-166">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="2d04f-167">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="2d04f-167">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="2d04f-168">status</span><span class="sxs-lookup"><span data-stu-id="2d04f-168">status</span></span>|<span data-ttu-id="2d04f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d04f-169">String</span></span>|<span data-ttu-id="2d04f-170">O estado do ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="2d04f-170">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="2d04f-171">Os estados possíveis **são InDevelopment,** **Available** e **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="2d04f-171">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="2d04f-172">Definir automaticamente **como InDevelopment na** criação.</span><span class="sxs-lookup"><span data-stu-id="2d04f-172">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="2d04f-173">[As extensões de esquema](/graph/extensibility-overview#schema-extensions) fornece mais informações sobre as possíveis transições de estado e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="2d04f-173">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span> <span data-ttu-id="2d04f-174">Suporta `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="2d04f-174">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="2d04f-175">targetTypes</span><span class="sxs-lookup"><span data-stu-id="2d04f-175">targetTypes</span></span>|<span data-ttu-id="2d04f-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d04f-176">String collection</span></span>|<span data-ttu-id="2d04f-177">Conjunto de tipos Graph microsoft (que podem dar suporte a extensões) aos quais a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="2d04f-177">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="2d04f-178">Selecione **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span><span class="sxs-lookup"><span data-stu-id="2d04f-178">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d04f-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d04f-179">JSON representation</span></span>

<span data-ttu-id="2d04f-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d04f-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


