---
title: Update schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 9f8bfc77ddcb3633160f76ce5d900e4ba09af1c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521079"
---
# <a name="update-schemaextension"></a><span data-ttu-id="357b7-103">Update schemaExtension</span><span class="sxs-lookup"><span data-stu-id="357b7-103">Update schemaExtension</span></span>

<span data-ttu-id="357b7-104">Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="357b7-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="357b7-105">A atualização se aplica a todos os recursos incluídos na propriedade **TargetTypes** da extensão.</span><span class="sxs-lookup"><span data-stu-id="357b7-105">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="357b7-106">Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="357b7-106">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="357b7-107">Somente o aplicativo que criou uma extensão de esquema (aplicativo proprietário) pode fazer atualizações aditivas para a extensão quando a extensão está \*\*\*\* no indesenvolvimento ou status **disponível** .</span><span class="sxs-lookup"><span data-stu-id="357b7-107">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="357b7-108">Isso significa que o aplicativo não pode remover propriedades personalizadas ou tipos de recurso de destino da definição.</span><span class="sxs-lookup"><span data-stu-id="357b7-108">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="357b7-109">No entanto, o aplicativo pode alterar a descrição da extensão.</span><span class="sxs-lookup"><span data-stu-id="357b7-109">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="357b7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="357b7-110">Permissions</span></span>
<span data-ttu-id="357b7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="357b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="357b7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="357b7-113">Permission type</span></span>      | <span data-ttu-id="357b7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="357b7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="357b7-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="357b7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="357b7-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="357b7-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="357b7-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="357b7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="357b7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357b7-118">Not supported.</span></span>    |
|<span data-ttu-id="357b7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="357b7-119">Application</span></span> | <span data-ttu-id="357b7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357b7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="357b7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="357b7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="357b7-122">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="357b7-122">Optional request headers</span></span>

| <span data-ttu-id="357b7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="357b7-123">Name</span></span>      |<span data-ttu-id="357b7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="357b7-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="357b7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="357b7-125">Authorization</span></span>  | <span data-ttu-id="357b7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="357b7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="357b7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="357b7-128">Content-Type</span></span>   | <span data-ttu-id="357b7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="357b7-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="357b7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="357b7-130">Request body</span></span>

<span data-ttu-id="357b7-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="357b7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="357b7-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="357b7-134">Property</span></span>   | <span data-ttu-id="357b7-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="357b7-135">Type</span></span> |<span data-ttu-id="357b7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="357b7-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="357b7-137">description</span><span class="sxs-lookup"><span data-stu-id="357b7-137">description</span></span>|<span data-ttu-id="357b7-138">String</span><span class="sxs-lookup"><span data-stu-id="357b7-138">String</span></span>|<span data-ttu-id="357b7-139">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="357b7-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="357b7-140">properties</span><span class="sxs-lookup"><span data-stu-id="357b7-140">properties</span></span>|<span data-ttu-id="357b7-141">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="357b7-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="357b7-142">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="357b7-142">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="357b7-143">Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="357b7-143">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="357b7-144">status</span><span class="sxs-lookup"><span data-stu-id="357b7-144">status</span></span>|<span data-ttu-id="357b7-145">String</span><span class="sxs-lookup"><span data-stu-id="357b7-145">String</span></span>|<span data-ttu-id="357b7-146">O estado do ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="357b7-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="357b7-147">O estado inicial na criação é \*\*\*\* o indevelopment.</span><span class="sxs-lookup"><span data-stu-id="357b7-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="357b7-148">Os possíveis transições de Estados \*\*\*\* estão de indevelopment para **Available** e **disponíveis** para preteridos. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="357b7-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="357b7-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="357b7-149">targetTypes</span></span>|<span data-ttu-id="357b7-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="357b7-150">String collection</span></span>|<span data-ttu-id="357b7-151">Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="357b7-151">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="357b7-152">Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="357b7-152">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="357b7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="357b7-153">Response</span></span>

<span data-ttu-id="357b7-154">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="357b7-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="357b7-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="357b7-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="357b7-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="357b7-156">Request</span></span>

<span data-ttu-id="357b7-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="357b7-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a><span data-ttu-id="357b7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="357b7-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="357b7-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="357b7-159">See also</span></span>

- [<span data-ttu-id="357b7-160">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="357b7-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="357b7-161">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="357b7-161">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
