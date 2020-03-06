---
title: Update schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c1e6e58c19f6561c16f51967a3b3a0c4ae346158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509938"
---
# <a name="update-schemaextension"></a><span data-ttu-id="20e57-103">Update schemaExtension</span><span class="sxs-lookup"><span data-stu-id="20e57-103">Update schemaExtension</span></span>

<span data-ttu-id="20e57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20e57-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20e57-105">Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="20e57-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="20e57-106">A atualização se aplica a todos os recursos incluídos na propriedade **TargetTypes** da extensão.</span><span class="sxs-lookup"><span data-stu-id="20e57-106">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="20e57-107">Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="20e57-107">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="20e57-108">Somente o aplicativo que criou uma extensão de esquema (aplicativo proprietário) pode fazer atualizações aditivas para a extensão quando a extensão está no **indesenvolvimento** ou status **disponível** .</span><span class="sxs-lookup"><span data-stu-id="20e57-108">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="20e57-109">Isso significa que o aplicativo não pode remover propriedades personalizadas ou tipos de recurso de destino da definição.</span><span class="sxs-lookup"><span data-stu-id="20e57-109">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="20e57-110">No entanto, o aplicativo pode alterar a descrição da extensão.</span><span class="sxs-lookup"><span data-stu-id="20e57-110">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="20e57-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="20e57-111">Permissions</span></span>
<span data-ttu-id="20e57-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e57-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="20e57-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20e57-114">Permission type</span></span>      | <span data-ttu-id="20e57-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20e57-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e57-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20e57-116">Delegated (work or school account)</span></span> | <span data-ttu-id="20e57-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20e57-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20e57-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20e57-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e57-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e57-119">Not supported.</span></span>    |
|<span data-ttu-id="20e57-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20e57-120">Application</span></span> | <span data-ttu-id="20e57-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e57-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e57-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20e57-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="20e57-123">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="20e57-123">Optional request headers</span></span>

| <span data-ttu-id="20e57-124">Nome</span><span class="sxs-lookup"><span data-stu-id="20e57-124">Name</span></span>      |<span data-ttu-id="20e57-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e57-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20e57-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="20e57-126">Authorization</span></span>  | <span data-ttu-id="20e57-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20e57-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20e57-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20e57-129">Content-Type</span></span>   | <span data-ttu-id="20e57-130">application/json</span><span class="sxs-lookup"><span data-stu-id="20e57-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="20e57-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20e57-131">Request body</span></span>

<span data-ttu-id="20e57-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="20e57-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="20e57-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20e57-135">Property</span></span>   | <span data-ttu-id="20e57-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="20e57-136">Type</span></span> |<span data-ttu-id="20e57-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e57-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20e57-138">description</span><span class="sxs-lookup"><span data-stu-id="20e57-138">description</span></span>|<span data-ttu-id="20e57-139">String</span><span class="sxs-lookup"><span data-stu-id="20e57-139">String</span></span>|<span data-ttu-id="20e57-140">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="20e57-140">Description for the schema extension.</span></span>|
|<span data-ttu-id="20e57-141">properties</span><span class="sxs-lookup"><span data-stu-id="20e57-141">properties</span></span>|<span data-ttu-id="20e57-142">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="20e57-142">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="20e57-143">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="20e57-143">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="20e57-144">Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="20e57-144">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="20e57-145">status</span><span class="sxs-lookup"><span data-stu-id="20e57-145">status</span></span>|<span data-ttu-id="20e57-146">String</span><span class="sxs-lookup"><span data-stu-id="20e57-146">String</span></span>|<span data-ttu-id="20e57-147">O estado do ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="20e57-147">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="20e57-148">O estado inicial na criação é o **indevelopment**.</span><span class="sxs-lookup"><span data-stu-id="20e57-148">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="20e57-149">Os possíveis transições de Estados estão de **indevelopment** para **Available** e **disponíveis** para **preteridos**.</span><span class="sxs-lookup"><span data-stu-id="20e57-149">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="20e57-150">targetTypes</span><span class="sxs-lookup"><span data-stu-id="20e57-150">targetTypes</span></span>|<span data-ttu-id="20e57-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e57-151">String collection</span></span>|<span data-ttu-id="20e57-152">Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="20e57-152">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="20e57-153">Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="20e57-153">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="20e57-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e57-154">Response</span></span>

<span data-ttu-id="20e57-155">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="20e57-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="20e57-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20e57-156">Example</span></span>

##### <a name="request"></a><span data-ttu-id="20e57-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20e57-157">Request</span></span>

<span data-ttu-id="20e57-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20e57-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20e57-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="20e57-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="20e57-160">C#</span><span class="sxs-lookup"><span data-stu-id="20e57-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20e57-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e57-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20e57-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20e57-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20e57-163">Java</span><span class="sxs-lookup"><span data-stu-id="20e57-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="20e57-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e57-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="20e57-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="20e57-165">See also</span></span>

- [<span data-ttu-id="20e57-166">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="20e57-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="20e57-167">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="20e57-167">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
