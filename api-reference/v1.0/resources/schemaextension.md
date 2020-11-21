---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: 728908089248e2b34eb09e0bbfbb7741146e86ae
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352330"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="5f33e-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="5f33e-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="5f33e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f33e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f33e-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="5f33e-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="5f33e-108">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="5f33e-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="5f33e-109">contact</span><span class="sxs-lookup"><span data-stu-id="5f33e-109">contact</span></span>](contact.md)
- [<span data-ttu-id="5f33e-110">device</span><span class="sxs-lookup"><span data-stu-id="5f33e-110">device</span></span>](device.md)
- <span data-ttu-id="5f33e-111">[event](event.md) em um usuário ou calendário de grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5f33e-111">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="5f33e-112">[post](post.md) de um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5f33e-112">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="5f33e-113">grupo</span><span class="sxs-lookup"><span data-stu-id="5f33e-113">group</span></span>](group.md)
- [<span data-ttu-id="5f33e-114">message</span><span class="sxs-lookup"><span data-stu-id="5f33e-114">message</span></span>](message.md) 
- [<span data-ttu-id="5f33e-115">organization</span><span class="sxs-lookup"><span data-stu-id="5f33e-115">organization</span></span>](organization.md)
- [<span data-ttu-id="5f33e-116">user</span><span class="sxs-lookup"><span data-stu-id="5f33e-116">user</span></span>](user.md)

<span data-ttu-id="5f33e-117">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="5f33e-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="5f33e-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="5f33e-118">Methods</span></span>

| <span data-ttu-id="5f33e-119">Método</span><span class="sxs-lookup"><span data-stu-id="5f33e-119">Method</span></span>           | <span data-ttu-id="5f33e-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5f33e-120">Return Type</span></span>    |<span data-ttu-id="5f33e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f33e-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f33e-122">Criar</span><span class="sxs-lookup"><span data-stu-id="5f33e-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="5f33e-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5f33e-123">schemaExtension</span></span> |<span data-ttu-id="5f33e-124">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="5f33e-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="5f33e-125">Listar</span><span class="sxs-lookup"><span data-stu-id="5f33e-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="5f33e-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5f33e-126">schemaExtension</span></span> |<span data-ttu-id="5f33e-127">Lista as definições de schemaExtension disponíveis e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="5f33e-127">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="5f33e-128">Get</span><span class="sxs-lookup"><span data-stu-id="5f33e-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="5f33e-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5f33e-129">schemaExtension</span></span> |<span data-ttu-id="5f33e-130">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="5f33e-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="5f33e-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="5f33e-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="5f33e-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5f33e-132">schemaExtension</span></span>   |<span data-ttu-id="5f33e-133">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="5f33e-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="5f33e-134">Excluir</span><span class="sxs-lookup"><span data-stu-id="5f33e-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="5f33e-135">None</span><span class="sxs-lookup"><span data-stu-id="5f33e-135">None</span></span> |<span data-ttu-id="5f33e-136">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="5f33e-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="5f33e-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f33e-137">Properties</span></span>
| <span data-ttu-id="5f33e-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f33e-138">Property</span></span>     | <span data-ttu-id="5f33e-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f33e-139">Type</span></span>   |<span data-ttu-id="5f33e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f33e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f33e-141">description</span><span class="sxs-lookup"><span data-stu-id="5f33e-141">description</span></span>|<span data-ttu-id="5f33e-142">String</span><span class="sxs-lookup"><span data-stu-id="5f33e-142">String</span></span>|<span data-ttu-id="5f33e-143">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="5f33e-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="5f33e-144">id</span><span class="sxs-lookup"><span data-stu-id="5f33e-144">id</span></span>|<span data-ttu-id="5f33e-145">String</span><span class="sxs-lookup"><span data-stu-id="5f33e-145">String</span></span>|<span data-ttu-id="5f33e-146">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="5f33e-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="5f33e-147">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="5f33e-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="5f33e-p103">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="5f33e-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="5f33e-p104">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="5f33e-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="5f33e-152">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="5f33e-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="5f33e-153">owner</span><span class="sxs-lookup"><span data-stu-id="5f33e-153">owner</span></span>|<span data-ttu-id="5f33e-154">String</span><span class="sxs-lookup"><span data-stu-id="5f33e-154">String</span></span>|<span data-ttu-id="5f33e-155">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="5f33e-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="5f33e-156">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="5f33e-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="5f33e-157">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="5f33e-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="5f33e-158">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5f33e-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="5f33e-159">Então, por exemplo, se criar uma nova definição de extensão do esquema usando o Explorador do Graph, você **deverá** fornecer a propriedade de proprietário.</span><span class="sxs-lookup"><span data-stu-id="5f33e-159">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="5f33e-160">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="5f33e-160">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="5f33e-161">properties</span><span class="sxs-lookup"><span data-stu-id="5f33e-161">properties</span></span>|<span data-ttu-id="5f33e-162">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5f33e-162">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="5f33e-163">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="5f33e-163">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="5f33e-164">status</span><span class="sxs-lookup"><span data-stu-id="5f33e-164">status</span></span>|<span data-ttu-id="5f33e-165">String</span><span class="sxs-lookup"><span data-stu-id="5f33e-165">String</span></span>|<span data-ttu-id="5f33e-p106">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="5f33e-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="5f33e-170">targetTypes</span><span class="sxs-lookup"><span data-stu-id="5f33e-170">targetTypes</span></span>|<span data-ttu-id="5f33e-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f33e-171">String collection</span></span>|<span data-ttu-id="5f33e-p107">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.</span><span class="sxs-lookup"><span data-stu-id="5f33e-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f33e-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f33e-174">JSON representation</span></span>

<span data-ttu-id="5f33e-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f33e-175">Here is a JSON representation of the resource.</span></span>

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

