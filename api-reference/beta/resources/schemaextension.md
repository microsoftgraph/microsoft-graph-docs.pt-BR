---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
localization_priority: Normal
ms.openlocfilehash: df0b362e87fa0f8cf836c27e89a5fdebd4ab0de8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894499"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="11bb3-104">Tipo de recurso schemaExtension (extensões de esquema)</span><span class="sxs-lookup"><span data-stu-id="11bb3-104">schemaExtension resource type (schema extensions)</span></span>

> <span data-ttu-id="11bb3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11bb3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11bb3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11bb3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11bb3-p103">As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido.</span><span class="sxs-lookup"><span data-stu-id="11bb3-p103">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="11bb3-109">As extensões de esquema são suportadas pelos seguintes tipos de recursos:</span><span class="sxs-lookup"><span data-stu-id="11bb3-109">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="11bb3-110">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="11bb3-110">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="11bb3-111">contact</span><span class="sxs-lookup"><span data-stu-id="11bb3-111">contact</span></span>](contact.md)
 - [<span data-ttu-id="11bb3-112">device</span><span class="sxs-lookup"><span data-stu-id="11bb3-112">device</span></span>](device.md)
 - <span data-ttu-id="11bb3-113">[event](event.md) em um usuário ou calendário de grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="11bb3-113">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="11bb3-114">[post](post.md) de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="11bb3-114">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="11bb3-115">group</span><span class="sxs-lookup"><span data-stu-id="11bb3-115">group</span></span>](group.md)
 - [<span data-ttu-id="11bb3-116">message</span><span class="sxs-lookup"><span data-stu-id="11bb3-116">message</span></span>](message.md) 
 - [<span data-ttu-id="11bb3-117">organization</span><span class="sxs-lookup"><span data-stu-id="11bb3-117">organization</span></span>](organization.md)
 - [<span data-ttu-id="11bb3-118">user</span><span class="sxs-lookup"><span data-stu-id="11bb3-118">user</span></span>](user.md)

<span data-ttu-id="11bb3-119">Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.</span><span class="sxs-lookup"><span data-stu-id="11bb3-119">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="11bb3-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="11bb3-120">Methods</span></span>

| <span data-ttu-id="11bb3-121">Método</span><span class="sxs-lookup"><span data-stu-id="11bb3-121">Method</span></span>           | <span data-ttu-id="11bb3-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11bb3-122">Return Type</span></span>    |<span data-ttu-id="11bb3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="11bb3-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11bb3-124">Criar</span><span class="sxs-lookup"><span data-stu-id="11bb3-124">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="11bb3-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="11bb3-125">schemaExtension</span></span> |<span data-ttu-id="11bb3-126">Crie uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="11bb3-126">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="11bb3-127">Listar</span><span class="sxs-lookup"><span data-stu-id="11bb3-127">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="11bb3-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="11bb3-128">schemaExtension</span></span> |<span data-ttu-id="11bb3-129">Liste as definições de schemaExtension avaialbe e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="11bb3-129">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="11bb3-130">Get</span><span class="sxs-lookup"><span data-stu-id="11bb3-130">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="11bb3-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="11bb3-131">schemaExtension</span></span> |<span data-ttu-id="11bb3-132">Leia as propriedades da definição de schemaExtension específica.</span><span class="sxs-lookup"><span data-stu-id="11bb3-132">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="11bb3-133">Atualizar</span><span class="sxs-lookup"><span data-stu-id="11bb3-133">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="11bb3-134">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="11bb3-134">schemaExtension</span></span>   |<span data-ttu-id="11bb3-135">Atualize uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="11bb3-135">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="11bb3-136">Excluir</span><span class="sxs-lookup"><span data-stu-id="11bb3-136">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="11bb3-137">None</span><span class="sxs-lookup"><span data-stu-id="11bb3-137">None</span></span> |<span data-ttu-id="11bb3-138">Exclua uma definição de schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="11bb3-138">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="11bb3-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11bb3-139">Properties</span></span>
| <span data-ttu-id="11bb3-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11bb3-140">Property</span></span>     | <span data-ttu-id="11bb3-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="11bb3-141">Type</span></span>   |<span data-ttu-id="11bb3-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="11bb3-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11bb3-143">description</span><span class="sxs-lookup"><span data-stu-id="11bb3-143">description</span></span>|<span data-ttu-id="11bb3-144">String</span><span class="sxs-lookup"><span data-stu-id="11bb3-144">String</span></span>|<span data-ttu-id="11bb3-145">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="11bb3-145">Description for the schema extension.</span></span>|
|<span data-ttu-id="11bb3-146">id</span><span class="sxs-lookup"><span data-stu-id="11bb3-146">id</span></span>|<span data-ttu-id="11bb3-147">String</span><span class="sxs-lookup"><span data-stu-id="11bb3-147">String</span></span>|<span data-ttu-id="11bb3-148">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="11bb3-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="11bb3-149">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="11bb3-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="11bb3-p104">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="11bb3-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="11bb3-p105">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="11bb3-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="11bb3-154">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="11bb3-154">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="11bb3-155">owner</span><span class="sxs-lookup"><span data-stu-id="11bb3-155">owner</span></span>|<span data-ttu-id="11bb3-156">String</span><span class="sxs-lookup"><span data-stu-id="11bb3-156">String</span></span>|<span data-ttu-id="11bb3-157">O `appId` do aplicativo que é o proprietário da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="11bb3-157">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="11bb3-158">Essa propriedade pode ser fornecida na criação, para definir o proprietário.</span><span class="sxs-lookup"><span data-stu-id="11bb3-158">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="11bb3-159">Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário.</span><span class="sxs-lookup"><span data-stu-id="11bb3-159">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="11bb3-160">Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11bb3-160">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="11bb3-161">Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="11bb3-161">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="11bb3-162">properties</span><span class="sxs-lookup"><span data-stu-id="11bb3-162">properties</span></span>|<span data-ttu-id="11bb3-163">Coleção [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="11bb3-163">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="11bb3-164">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="11bb3-164">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="11bb3-165">status</span><span class="sxs-lookup"><span data-stu-id="11bb3-165">status</span></span>|<span data-ttu-id="11bb3-166">String</span><span class="sxs-lookup"><span data-stu-id="11bb3-166">String</span></span>|<span data-ttu-id="11bb3-p107">O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.</span><span class="sxs-lookup"><span data-stu-id="11bb3-p107">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="11bb3-171">targetTypes</span><span class="sxs-lookup"><span data-stu-id="11bb3-171">targetTypes</span></span>|<span data-ttu-id="11bb3-172">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11bb3-172">String collection</span></span>|<span data-ttu-id="11bb3-173">Conjunto de tipos do Microsoft Graph (que podem suportar extensões) que a extensão do esquema pode ser aplicada a.</span><span class="sxs-lookup"><span data-stu-id="11bb3-173">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="11bb3-174">Selecione **administrativeUnit**, **entre em contato**, **dispositivo**, **evento**, **grupo**, **mensagem**, **organização**, **postar**ou **usuário**.</span><span class="sxs-lookup"><span data-stu-id="11bb3-174">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11bb3-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11bb3-175">JSON representation</span></span>

<span data-ttu-id="11bb3-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11bb3-176">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
