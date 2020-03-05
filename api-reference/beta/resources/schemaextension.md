---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 79cac458ed09663e3bdf9c07aefb7408d46e05cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520946"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="124e1-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="124e1-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="124e1-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="124e1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="124e1-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="124e1-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="124e1-108">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="124e1-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="124e1-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="124e1-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="124e1-110">contact</span><span class="sxs-lookup"><span data-stu-id="124e1-110">contact</span></span>](contact.md)
- [<span data-ttu-id="124e1-111">device</span><span class="sxs-lookup"><span data-stu-id="124e1-111">device</span></span>](device.md)
- <span data-ttu-id="124e1-112">[event](event.md) em um usuário ou calendário de grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="124e1-112">[event](event.md) on a user or Office 365 group calendar</span></span>
- <span data-ttu-id="124e1-113">[post](post.md) de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="124e1-113">[post](post.md) of an Office 365 group</span></span>
- [<span data-ttu-id="124e1-114">group</span><span class="sxs-lookup"><span data-stu-id="124e1-114">group</span></span>](group.md)
- [<span data-ttu-id="124e1-115">message</span><span class="sxs-lookup"><span data-stu-id="124e1-115">message</span></span>](message.md) 
- [<span data-ttu-id="124e1-116">organization</span><span class="sxs-lookup"><span data-stu-id="124e1-116">organization</span></span>](organization.md)
- [<span data-ttu-id="124e1-117">user</span><span class="sxs-lookup"><span data-stu-id="124e1-117">user</span></span>](user.md)

<span data-ttu-id="124e1-118">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="124e1-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="124e1-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="124e1-119">Methods</span></span>

| <span data-ttu-id="124e1-120">Método</span><span class="sxs-lookup"><span data-stu-id="124e1-120">Method</span></span>           | <span data-ttu-id="124e1-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="124e1-121">Return Type</span></span>    |<span data-ttu-id="124e1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="124e1-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="124e1-123">Criar</span><span class="sxs-lookup"><span data-stu-id="124e1-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="124e1-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="124e1-124">schemaExtension</span></span> |<span data-ttu-id="124e1-125">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="124e1-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="124e1-126">Listar</span><span class="sxs-lookup"><span data-stu-id="124e1-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="124e1-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="124e1-127">schemaExtension</span></span> |<span data-ttu-id="124e1-128">Liste a avaialbe schemaExtension defintions e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="124e1-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="124e1-129">Get</span><span class="sxs-lookup"><span data-stu-id="124e1-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="124e1-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="124e1-130">schemaExtension</span></span> |<span data-ttu-id="124e1-131">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="124e1-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="124e1-132">Atualizar</span><span class="sxs-lookup"><span data-stu-id="124e1-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="124e1-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="124e1-133">schemaExtension</span></span>   |<span data-ttu-id="124e1-134">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="124e1-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="124e1-135">Excluir</span><span class="sxs-lookup"><span data-stu-id="124e1-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="124e1-136">None</span><span class="sxs-lookup"><span data-stu-id="124e1-136">None</span></span> |<span data-ttu-id="124e1-137">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="124e1-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="124e1-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="124e1-138">Properties</span></span>
| <span data-ttu-id="124e1-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="124e1-139">Property</span></span>     | <span data-ttu-id="124e1-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="124e1-140">Type</span></span>   |<span data-ttu-id="124e1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="124e1-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="124e1-142">description</span><span class="sxs-lookup"><span data-stu-id="124e1-142">description</span></span>|<span data-ttu-id="124e1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="124e1-143">String</span></span>|<span data-ttu-id="124e1-144">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="124e1-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="124e1-145">id</span><span class="sxs-lookup"><span data-stu-id="124e1-145">id</span></span>|<span data-ttu-id="124e1-146">String</span><span class="sxs-lookup"><span data-stu-id="124e1-146">String</span></span>|<span data-ttu-id="124e1-147">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="124e1-147">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="124e1-148">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="124e1-148">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="124e1-p103">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="124e1-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="124e1-p104">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="124e1-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="124e1-153">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="124e1-153">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="124e1-154">owner</span><span class="sxs-lookup"><span data-stu-id="124e1-154">owner</span></span>|<span data-ttu-id="124e1-155">String</span><span class="sxs-lookup"><span data-stu-id="124e1-155">String</span></span>|<span data-ttu-id="124e1-156">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="124e1-156">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="124e1-157">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="124e1-157">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="124e1-158">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="124e1-158">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="124e1-159">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="124e1-159">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="124e1-160">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="124e1-160">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="124e1-161">properties</span><span class="sxs-lookup"><span data-stu-id="124e1-161">properties</span></span>|<span data-ttu-id="124e1-162">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="124e1-162">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="124e1-163">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="124e1-163">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="124e1-164">status</span><span class="sxs-lookup"><span data-stu-id="124e1-164">status</span></span>|<span data-ttu-id="124e1-165">String</span><span class="sxs-lookup"><span data-stu-id="124e1-165">String</span></span>|<span data-ttu-id="124e1-p106">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="124e1-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="124e1-170">targetTypes</span><span class="sxs-lookup"><span data-stu-id="124e1-170">targetTypes</span></span>|<span data-ttu-id="124e1-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="124e1-171">String collection</span></span>|<span data-ttu-id="124e1-172">Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="124e1-172">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="124e1-173">Selecione entre **administrativeUnit**, **contato**, **dispositivo**, **evento**, **grupo**, **mensagem**, **organização**, **postagem**ou **usuário**.</span><span class="sxs-lookup"><span data-stu-id="124e1-173">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="124e1-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="124e1-174">JSON representation</span></span>

<span data-ttu-id="124e1-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="124e1-175">Here is a JSON representation of the resource.</span></span>

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
