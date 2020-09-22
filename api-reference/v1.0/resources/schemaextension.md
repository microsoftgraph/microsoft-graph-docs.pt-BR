---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: 71c4bd70fafe2ea652d2a0e31134196281aa161d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984149"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="0cf49-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="0cf49-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="0cf49-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf49-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cf49-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="0cf49-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="0cf49-108">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="0cf49-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="0cf49-109">contact</span><span class="sxs-lookup"><span data-stu-id="0cf49-109">contact</span></span>](contact.md)
- [<span data-ttu-id="0cf49-110">device</span><span class="sxs-lookup"><span data-stu-id="0cf49-110">device</span></span>](device.md)
- <span data-ttu-id="0cf49-111">[event](event.md) em um usuário ou calendário de grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0cf49-111">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="0cf49-112">[post](post.md) de um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0cf49-112">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="0cf49-113">grupo</span><span class="sxs-lookup"><span data-stu-id="0cf49-113">group</span></span>](group.md)
- [<span data-ttu-id="0cf49-114">message</span><span class="sxs-lookup"><span data-stu-id="0cf49-114">message</span></span>](message.md) 
- [<span data-ttu-id="0cf49-115">organization</span><span class="sxs-lookup"><span data-stu-id="0cf49-115">organization</span></span>](organization.md)
- [<span data-ttu-id="0cf49-116">user</span><span class="sxs-lookup"><span data-stu-id="0cf49-116">user</span></span>](user.md)

<span data-ttu-id="0cf49-117">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="0cf49-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="0cf49-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="0cf49-118">Methods</span></span>

| <span data-ttu-id="0cf49-119">Método</span><span class="sxs-lookup"><span data-stu-id="0cf49-119">Method</span></span>           | <span data-ttu-id="0cf49-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0cf49-120">Return Type</span></span>    |<span data-ttu-id="0cf49-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf49-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cf49-122">Criar</span><span class="sxs-lookup"><span data-stu-id="0cf49-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="0cf49-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0cf49-123">schemaExtension</span></span> |<span data-ttu-id="0cf49-124">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="0cf49-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="0cf49-125">Listar</span><span class="sxs-lookup"><span data-stu-id="0cf49-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="0cf49-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0cf49-126">schemaExtension</span></span> |<span data-ttu-id="0cf49-127">Lista as definições de schemaExtension disponíveis e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0cf49-127">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="0cf49-128">Get</span><span class="sxs-lookup"><span data-stu-id="0cf49-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="0cf49-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0cf49-129">schemaExtension</span></span> |<span data-ttu-id="0cf49-130">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="0cf49-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="0cf49-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="0cf49-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="0cf49-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0cf49-132">schemaExtension</span></span>   |<span data-ttu-id="0cf49-133">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="0cf49-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="0cf49-134">Excluir</span><span class="sxs-lookup"><span data-stu-id="0cf49-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="0cf49-135">None</span><span class="sxs-lookup"><span data-stu-id="0cf49-135">None</span></span> |<span data-ttu-id="0cf49-136">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="0cf49-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="0cf49-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cf49-137">Properties</span></span>
| <span data-ttu-id="0cf49-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cf49-138">Property</span></span>     | <span data-ttu-id="0cf49-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cf49-139">Type</span></span>   |<span data-ttu-id="0cf49-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf49-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cf49-141">description</span><span class="sxs-lookup"><span data-stu-id="0cf49-141">description</span></span>|<span data-ttu-id="0cf49-142">String</span><span class="sxs-lookup"><span data-stu-id="0cf49-142">String</span></span>|<span data-ttu-id="0cf49-143">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="0cf49-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="0cf49-144">id</span><span class="sxs-lookup"><span data-stu-id="0cf49-144">id</span></span>|<span data-ttu-id="0cf49-145">String</span><span class="sxs-lookup"><span data-stu-id="0cf49-145">String</span></span>|<span data-ttu-id="0cf49-146">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="0cf49-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="0cf49-147">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="0cf49-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="0cf49-p103">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="0cf49-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="0cf49-p104">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="0cf49-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="0cf49-152">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="0cf49-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="0cf49-153">owner</span><span class="sxs-lookup"><span data-stu-id="0cf49-153">owner</span></span>|<span data-ttu-id="0cf49-154">String</span><span class="sxs-lookup"><span data-stu-id="0cf49-154">String</span></span>|<span data-ttu-id="0cf49-155">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="0cf49-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="0cf49-156">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="0cf49-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="0cf49-157">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="0cf49-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="0cf49-158">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0cf49-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="0cf49-159">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="0cf49-159">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="0cf49-160">properties</span><span class="sxs-lookup"><span data-stu-id="0cf49-160">properties</span></span>|<span data-ttu-id="0cf49-161">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0cf49-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="0cf49-162">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="0cf49-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="0cf49-163">status</span><span class="sxs-lookup"><span data-stu-id="0cf49-163">status</span></span>|<span data-ttu-id="0cf49-164">String</span><span class="sxs-lookup"><span data-stu-id="0cf49-164">String</span></span>|<span data-ttu-id="0cf49-p106">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="0cf49-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="0cf49-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="0cf49-169">targetTypes</span></span>|<span data-ttu-id="0cf49-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf49-170">String collection</span></span>|<span data-ttu-id="0cf49-p107">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.</span><span class="sxs-lookup"><span data-stu-id="0cf49-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cf49-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cf49-173">JSON representation</span></span>

<span data-ttu-id="0cf49-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cf49-174">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

