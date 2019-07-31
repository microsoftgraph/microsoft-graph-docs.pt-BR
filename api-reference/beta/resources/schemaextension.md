---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e713426a09132828e9d4016c42e210b16852b03a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008632"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="02fe5-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="02fe5-104">schemaExtension resource type (schema extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02fe5-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="02fe5-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="02fe5-107">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="02fe5-107">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="02fe5-108">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="02fe5-108">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="02fe5-109">contact</span><span class="sxs-lookup"><span data-stu-id="02fe5-109">contact</span></span>](contact.md)
- [<span data-ttu-id="02fe5-110">device</span><span class="sxs-lookup"><span data-stu-id="02fe5-110">device</span></span>](device.md)
- <span data-ttu-id="02fe5-111">[event](event.md) em um usuário ou calendário de grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="02fe5-111">[event](event.md) on a user or Office 365 group calendar</span></span>
- <span data-ttu-id="02fe5-112">[post](post.md) de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="02fe5-112">[post](post.md) of an Office 365 group</span></span>
- [<span data-ttu-id="02fe5-113">group</span><span class="sxs-lookup"><span data-stu-id="02fe5-113">group</span></span>](group.md)
- [<span data-ttu-id="02fe5-114">message</span><span class="sxs-lookup"><span data-stu-id="02fe5-114">message</span></span>](message.md) 
- [<span data-ttu-id="02fe5-115">organization</span><span class="sxs-lookup"><span data-stu-id="02fe5-115">organization</span></span>](organization.md)
- [<span data-ttu-id="02fe5-116">user</span><span class="sxs-lookup"><span data-stu-id="02fe5-116">user</span></span>](user.md)

<span data-ttu-id="02fe5-117">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="02fe5-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="02fe5-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="02fe5-118">Methods</span></span>

| <span data-ttu-id="02fe5-119">Método</span><span class="sxs-lookup"><span data-stu-id="02fe5-119">Method</span></span>           | <span data-ttu-id="02fe5-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02fe5-120">Return Type</span></span>    |<span data-ttu-id="02fe5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fe5-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02fe5-122">Criar</span><span class="sxs-lookup"><span data-stu-id="02fe5-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="02fe5-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="02fe5-123">schemaExtension</span></span> |<span data-ttu-id="02fe5-124">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="02fe5-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="02fe5-125">Listar</span><span class="sxs-lookup"><span data-stu-id="02fe5-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="02fe5-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="02fe5-126">schemaExtension</span></span> |<span data-ttu-id="02fe5-127">Liste a avaialbe schemaExtension defintions e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="02fe5-127">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="02fe5-128">Get</span><span class="sxs-lookup"><span data-stu-id="02fe5-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="02fe5-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="02fe5-129">schemaExtension</span></span> |<span data-ttu-id="02fe5-130">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="02fe5-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="02fe5-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="02fe5-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="02fe5-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="02fe5-132">schemaExtension</span></span>   |<span data-ttu-id="02fe5-133">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="02fe5-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="02fe5-134">Excluir</span><span class="sxs-lookup"><span data-stu-id="02fe5-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="02fe5-135">None</span><span class="sxs-lookup"><span data-stu-id="02fe5-135">None</span></span> |<span data-ttu-id="02fe5-136">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="02fe5-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="02fe5-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02fe5-137">Properties</span></span>
| <span data-ttu-id="02fe5-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02fe5-138">Property</span></span>     | <span data-ttu-id="02fe5-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fe5-139">Type</span></span>   |<span data-ttu-id="02fe5-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fe5-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02fe5-141">description</span><span class="sxs-lookup"><span data-stu-id="02fe5-141">description</span></span>|<span data-ttu-id="02fe5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fe5-142">String</span></span>|<span data-ttu-id="02fe5-143">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="02fe5-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="02fe5-144">id</span><span class="sxs-lookup"><span data-stu-id="02fe5-144">id</span></span>|<span data-ttu-id="02fe5-145">String</span><span class="sxs-lookup"><span data-stu-id="02fe5-145">String</span></span>|<span data-ttu-id="02fe5-146">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="02fe5-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="02fe5-147">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="02fe5-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="02fe5-p103">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="02fe5-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="02fe5-p104">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="02fe5-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="02fe5-152">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="02fe5-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="02fe5-153">owner</span><span class="sxs-lookup"><span data-stu-id="02fe5-153">owner</span></span>|<span data-ttu-id="02fe5-154">String</span><span class="sxs-lookup"><span data-stu-id="02fe5-154">String</span></span>|<span data-ttu-id="02fe5-155">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="02fe5-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="02fe5-156">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="02fe5-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="02fe5-157">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="02fe5-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="02fe5-158">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02fe5-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="02fe5-159">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="02fe5-159">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="02fe5-160">properties</span><span class="sxs-lookup"><span data-stu-id="02fe5-160">properties</span></span>|<span data-ttu-id="02fe5-161">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="02fe5-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="02fe5-162">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="02fe5-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="02fe5-163">status</span><span class="sxs-lookup"><span data-stu-id="02fe5-163">status</span></span>|<span data-ttu-id="02fe5-164">String</span><span class="sxs-lookup"><span data-stu-id="02fe5-164">String</span></span>|<span data-ttu-id="02fe5-p106">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="02fe5-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="02fe5-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="02fe5-169">targetTypes</span></span>|<span data-ttu-id="02fe5-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fe5-170">String collection</span></span>|<span data-ttu-id="02fe5-171">Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="02fe5-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="02fe5-172">Selecione entre **administrativeUnit**, **contato**, **dispositivo**, **evento**, **grupo**, **mensagem**, **organização**, **postagem**ou **usuário**.</span><span class="sxs-lookup"><span data-stu-id="02fe5-172">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02fe5-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02fe5-173">JSON representation</span></span>

<span data-ttu-id="02fe5-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02fe5-174">Here is a JSON representation of the resource.</span></span>

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
