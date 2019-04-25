---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Priority
author: dkershaw10
ms.openlocfilehash: 64c9fa09b83af23604bf8a6e550533b259f1b0a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579223"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="094a3-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="094a3-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="094a3-p102">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="094a3-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="094a3-107">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="094a3-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="094a3-108">contact</span><span class="sxs-lookup"><span data-stu-id="094a3-108">contact</span></span>](contact.md)
 - [<span data-ttu-id="094a3-109">device</span><span class="sxs-lookup"><span data-stu-id="094a3-109">device</span></span>](device.md)
 - <span data-ttu-id="094a3-110">[event](event.md) em um usuário ou calendário de grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="094a3-110">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="094a3-111">[post](post.md) de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="094a3-111">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="094a3-112">group</span><span class="sxs-lookup"><span data-stu-id="094a3-112">group</span></span>](group.md)
 - [<span data-ttu-id="094a3-113">message</span><span class="sxs-lookup"><span data-stu-id="094a3-113">message</span></span>](message.md) 
 - [<span data-ttu-id="094a3-114">organization</span><span class="sxs-lookup"><span data-stu-id="094a3-114">organization</span></span>](organization.md)
 - [<span data-ttu-id="094a3-115">user</span><span class="sxs-lookup"><span data-stu-id="094a3-115">user</span></span>](user.md)

<span data-ttu-id="094a3-116">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="094a3-116">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="094a3-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="094a3-117">Methods</span></span>

| <span data-ttu-id="094a3-118">Método</span><span class="sxs-lookup"><span data-stu-id="094a3-118">Method</span></span>           | <span data-ttu-id="094a3-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="094a3-119">Return Type</span></span>    |<span data-ttu-id="094a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="094a3-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="094a3-121">Criar</span><span class="sxs-lookup"><span data-stu-id="094a3-121">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="094a3-122">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="094a3-122">schemaExtension</span></span> |<span data-ttu-id="094a3-123">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="094a3-123">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="094a3-124">Listar</span><span class="sxs-lookup"><span data-stu-id="094a3-124">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="094a3-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="094a3-125">schemaExtension</span></span> |<span data-ttu-id="094a3-126">Lista as definições de schemaExtension disponíveis e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="094a3-126">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="094a3-127">Get</span><span class="sxs-lookup"><span data-stu-id="094a3-127">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="094a3-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="094a3-128">schemaExtension</span></span> |<span data-ttu-id="094a3-129">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="094a3-129">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="094a3-130">Atualizar</span><span class="sxs-lookup"><span data-stu-id="094a3-130">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="094a3-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="094a3-131">schemaExtension</span></span>   |<span data-ttu-id="094a3-132">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="094a3-132">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="094a3-133">Excluir</span><span class="sxs-lookup"><span data-stu-id="094a3-133">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="094a3-134">None</span><span class="sxs-lookup"><span data-stu-id="094a3-134">None</span></span> |<span data-ttu-id="094a3-135">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="094a3-135">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="094a3-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="094a3-136">Properties</span></span>
| <span data-ttu-id="094a3-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="094a3-137">Property</span></span>     | <span data-ttu-id="094a3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="094a3-138">Type</span></span>   |<span data-ttu-id="094a3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="094a3-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="094a3-140">description</span><span class="sxs-lookup"><span data-stu-id="094a3-140">description</span></span>|<span data-ttu-id="094a3-141">String</span><span class="sxs-lookup"><span data-stu-id="094a3-141">String</span></span>|<span data-ttu-id="094a3-142">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="094a3-142">Description for the schema extension.</span></span>|
|<span data-ttu-id="094a3-143">id</span><span class="sxs-lookup"><span data-stu-id="094a3-143">id</span></span>|<span data-ttu-id="094a3-144">String</span><span class="sxs-lookup"><span data-stu-id="094a3-144">String</span></span>|<span data-ttu-id="094a3-145">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="094a3-145">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="094a3-146">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="094a3-146">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="094a3-p103">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="094a3-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="094a3-p104">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="094a3-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="094a3-151">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="094a3-151">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="094a3-152">owner</span><span class="sxs-lookup"><span data-stu-id="094a3-152">owner</span></span>|<span data-ttu-id="094a3-153">String</span><span class="sxs-lookup"><span data-stu-id="094a3-153">String</span></span>|<span data-ttu-id="094a3-154">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="094a3-154">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="094a3-155">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="094a3-155">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="094a3-156">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="094a3-156">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="094a3-157">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="094a3-157">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="094a3-158">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="094a3-158">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="094a3-159">properties</span><span class="sxs-lookup"><span data-stu-id="094a3-159">properties</span></span>|<span data-ttu-id="094a3-160">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="094a3-160">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="094a3-161">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="094a3-161">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="094a3-162">status</span><span class="sxs-lookup"><span data-stu-id="094a3-162">status</span></span>|<span data-ttu-id="094a3-163">String</span><span class="sxs-lookup"><span data-stu-id="094a3-163">String</span></span>|<span data-ttu-id="094a3-p106">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="094a3-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="094a3-168">targetTypes</span><span class="sxs-lookup"><span data-stu-id="094a3-168">targetTypes</span></span>|<span data-ttu-id="094a3-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="094a3-169">String collection</span></span>|<span data-ttu-id="094a3-p107">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.</span><span class="sxs-lookup"><span data-stu-id="094a3-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="094a3-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="094a3-172">JSON representation</span></span>

<span data-ttu-id="094a3-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="094a3-173">Here is a JSON representation of the resource.</span></span>

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
