---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Priority
author: dkershaw10
ms.openlocfilehash: 72260112e2b23bf185ea86d039fec9e0af778fb9
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778345"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="42c6f-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="42c6f-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="42c6f-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="42c6f-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="42c6f-107">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="42c6f-107">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="42c6f-108">contact</span><span class="sxs-lookup"><span data-stu-id="42c6f-108">contact</span></span>](contact.md)
- [<span data-ttu-id="42c6f-109">device</span><span class="sxs-lookup"><span data-stu-id="42c6f-109">device</span></span>](device.md)
- <span data-ttu-id="42c6f-110">[event](event.md) em um usuário ou calendário de grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="42c6f-110">[event](event.md) on a user or Office 365 group calendar</span></span>
- <span data-ttu-id="42c6f-111">[post](post.md) de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="42c6f-111">[post](post.md) of an Office 365 group</span></span>
- [<span data-ttu-id="42c6f-112">group</span><span class="sxs-lookup"><span data-stu-id="42c6f-112">group</span></span>](group.md)
- [<span data-ttu-id="42c6f-113">message</span><span class="sxs-lookup"><span data-stu-id="42c6f-113">message</span></span>](message.md) 
- [<span data-ttu-id="42c6f-114">organization</span><span class="sxs-lookup"><span data-stu-id="42c6f-114">organization</span></span>](organization.md)
- [<span data-ttu-id="42c6f-115">user</span><span class="sxs-lookup"><span data-stu-id="42c6f-115">user</span></span>](user.md)

<span data-ttu-id="42c6f-116">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="42c6f-116">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="42c6f-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="42c6f-117">Methods</span></span>

| <span data-ttu-id="42c6f-118">Método</span><span class="sxs-lookup"><span data-stu-id="42c6f-118">Method</span></span>           | <span data-ttu-id="42c6f-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="42c6f-119">Return Type</span></span>    |<span data-ttu-id="42c6f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42c6f-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42c6f-121">Criar</span><span class="sxs-lookup"><span data-stu-id="42c6f-121">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="42c6f-122">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42c6f-122">schemaExtension</span></span> |<span data-ttu-id="42c6f-123">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="42c6f-123">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="42c6f-124">Listar</span><span class="sxs-lookup"><span data-stu-id="42c6f-124">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="42c6f-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42c6f-125">schemaExtension</span></span> |<span data-ttu-id="42c6f-126">Lista as definições de schemaExtension disponíveis e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="42c6f-126">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="42c6f-127">Get</span><span class="sxs-lookup"><span data-stu-id="42c6f-127">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="42c6f-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42c6f-128">schemaExtension</span></span> |<span data-ttu-id="42c6f-129">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="42c6f-129">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="42c6f-130">Atualizar</span><span class="sxs-lookup"><span data-stu-id="42c6f-130">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="42c6f-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42c6f-131">schemaExtension</span></span>   |<span data-ttu-id="42c6f-132">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="42c6f-132">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="42c6f-133">Excluir</span><span class="sxs-lookup"><span data-stu-id="42c6f-133">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="42c6f-134">None</span><span class="sxs-lookup"><span data-stu-id="42c6f-134">None</span></span> |<span data-ttu-id="42c6f-135">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="42c6f-135">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="42c6f-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42c6f-136">Properties</span></span>
| <span data-ttu-id="42c6f-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42c6f-137">Property</span></span>     | <span data-ttu-id="42c6f-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="42c6f-138">Type</span></span>   |<span data-ttu-id="42c6f-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="42c6f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42c6f-140">description</span><span class="sxs-lookup"><span data-stu-id="42c6f-140">description</span></span>|<span data-ttu-id="42c6f-141">String</span><span class="sxs-lookup"><span data-stu-id="42c6f-141">String</span></span>|<span data-ttu-id="42c6f-142">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="42c6f-142">Description for the schema extension.</span></span>|
|<span data-ttu-id="42c6f-143">id</span><span class="sxs-lookup"><span data-stu-id="42c6f-143">id</span></span>|<span data-ttu-id="42c6f-144">String</span><span class="sxs-lookup"><span data-stu-id="42c6f-144">String</span></span>|<span data-ttu-id="42c6f-145">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="42c6f-145">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="42c6f-146">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="42c6f-146">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="42c6f-p103">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="42c6f-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="42c6f-p104">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="42c6f-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="42c6f-151">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="42c6f-151">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="42c6f-152">owner</span><span class="sxs-lookup"><span data-stu-id="42c6f-152">owner</span></span>|<span data-ttu-id="42c6f-153">String</span><span class="sxs-lookup"><span data-stu-id="42c6f-153">String</span></span>|<span data-ttu-id="42c6f-154">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="42c6f-154">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="42c6f-155">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="42c6f-155">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="42c6f-156">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="42c6f-156">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="42c6f-157">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42c6f-157">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="42c6f-158">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="42c6f-158">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="42c6f-159">properties</span><span class="sxs-lookup"><span data-stu-id="42c6f-159">properties</span></span>|<span data-ttu-id="42c6f-160">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="42c6f-160">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="42c6f-161">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="42c6f-161">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="42c6f-162">status</span><span class="sxs-lookup"><span data-stu-id="42c6f-162">status</span></span>|<span data-ttu-id="42c6f-163">String</span><span class="sxs-lookup"><span data-stu-id="42c6f-163">String</span></span>|<span data-ttu-id="42c6f-p106">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="42c6f-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="42c6f-168">targetTypes</span><span class="sxs-lookup"><span data-stu-id="42c6f-168">targetTypes</span></span>|<span data-ttu-id="42c6f-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42c6f-169">String collection</span></span>|<span data-ttu-id="42c6f-p107">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.</span><span class="sxs-lookup"><span data-stu-id="42c6f-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42c6f-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42c6f-172">JSON representation</span></span>

<span data-ttu-id="42c6f-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42c6f-173">Here is a JSON representation of the resource.</span></span>

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
