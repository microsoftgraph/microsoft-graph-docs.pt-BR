---
title: Update schemaExtension
description: Atualizar propriedades na definição do esquemaExtension especificado.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 6e5bef7a1ac978ccde1c84a9ee074d7fc6d91c28
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787371"
---
# <a name="update-schemaextension"></a><span data-ttu-id="fcca5-103">Update schemaExtension</span><span class="sxs-lookup"><span data-stu-id="fcca5-103">Update schemaExtension</span></span>

<span data-ttu-id="fcca5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcca5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcca5-105">Atualizar propriedades na definição do [esquemaExtension especificado.](../resources/schemaextension.md)</span><span class="sxs-lookup"><span data-stu-id="fcca5-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span> <span data-ttu-id="fcca5-106">Atualizações aditivas para a extensão só podem ser feitas quando a extensão estiver no status **InDevelopment** ou **Disponível.**</span><span class="sxs-lookup"><span data-stu-id="fcca5-106">Additive updates to the extension can only be made when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="fcca5-107">Isso significa que propriedades personalizadas ou tipos de recurso de destino não podem ser removidos da definição, mas novas propriedades personalizadas podem ser adicionadas e a descrição da extensão alterada.</span><span class="sxs-lookup"><span data-stu-id="fcca5-107">This means custom properties or target resource types cannot be removed from the definition, but new custom properties can be added and the description of the extension changed.</span></span>

<span data-ttu-id="fcca5-108">A atualização se aplica a todos os recursos incluídos na **propriedade targetTypes** da extensão.</span><span class="sxs-lookup"><span data-stu-id="fcca5-108">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="fcca5-109">Esses recursos estão entre os [tipos de recursos de suporte.](/graph/extensibility-overview#supported-resources)</span><span class="sxs-lookup"><span data-stu-id="fcca5-109">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="fcca5-110">Para fluxos delegados, o usuário inscreveu pode atualizar  uma extensão de esquema desde que a propriedade proprietária da extensão seja definida como **appId** de um aplicativo que o usuário de entrada possui.</span><span class="sxs-lookup"><span data-stu-id="fcca5-110">For delegated flows, the signed-in user can update a schema extension as long as the **owner** property of the extension is set to the **appId** of an application the signed-in user owns.</span></span> <span data-ttu-id="fcca5-111">Esse aplicativo pode ser aquele que inicialmente criou a extensão ou algum outro aplicativo pertencente ao usuário in-locar.</span><span class="sxs-lookup"><span data-stu-id="fcca5-111">That application can be the one that initially created the extension, or some other application owned by the signed-in user.</span></span> 

<span data-ttu-id="fcca5-112">Esse critério para a propriedade **owner** permite que um usuário in-loco faça atualizações por meio de outros aplicativos que eles não têm, como o Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="fcca5-112">This criteria for the **owner** property allows a signed-in user to make updates through other applications they don't own, such as Microsoft Graph Explorer.</span></span> <span data-ttu-id="fcca5-113">Ao usar Graph Explorer para atualizar um recurso **schemaExtension,** inclua a propriedade **owner** no corpo da solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="fcca5-113">When using Graph Explorer to update a **schemaExtension** resource, include the **owner** property in the PATCH request body.</span></span> <span data-ttu-id="fcca5-114">Para obter mais informações, consulte a seção [Extensões](/graph/known-issues#extensions) em [Problemas conhecidos com a Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="fcca5-114">For more information, see the [Extensions](/graph/known-issues#extensions) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="fcca5-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="fcca5-115">Permissions</span></span>

<span data-ttu-id="fcca5-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcca5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fcca5-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcca5-118">Permission type</span></span>      | <span data-ttu-id="fcca5-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcca5-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcca5-120">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcca5-120">Delegated (work or school account)</span></span> | <span data-ttu-id="fcca5-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fcca5-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fcca5-122">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcca5-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcca5-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcca5-123">Not supported.</span></span>    |
|<span data-ttu-id="fcca5-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcca5-124">Application</span></span> | <span data-ttu-id="fcca5-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcca5-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcca5-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcca5-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="fcca5-127">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="fcca5-127">Optional request headers</span></span>

| <span data-ttu-id="fcca5-128">Nome</span><span class="sxs-lookup"><span data-stu-id="fcca5-128">Name</span></span>      |<span data-ttu-id="fcca5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcca5-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fcca5-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcca5-130">Authorization</span></span>  | <span data-ttu-id="fcca5-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcca5-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcca5-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcca5-133">Content-Type</span></span>   | <span data-ttu-id="fcca5-134">application/json</span><span class="sxs-lookup"><span data-stu-id="fcca5-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcca5-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcca5-135">Request body</span></span>

<span data-ttu-id="fcca5-p107">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fcca5-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fcca5-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcca5-139">Property</span></span>   | <span data-ttu-id="fcca5-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcca5-140">Type</span></span> |<span data-ttu-id="fcca5-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcca5-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcca5-142">description</span><span class="sxs-lookup"><span data-stu-id="fcca5-142">description</span></span>|<span data-ttu-id="fcca5-143">String</span><span class="sxs-lookup"><span data-stu-id="fcca5-143">String</span></span>|<span data-ttu-id="fcca5-144">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="fcca5-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="fcca5-145">properties</span><span class="sxs-lookup"><span data-stu-id="fcca5-145">properties</span></span>|<span data-ttu-id="fcca5-146">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="fcca5-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="fcca5-147">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="fcca5-147">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="fcca5-148">Somente alterações aditiva são permitidas.</span><span class="sxs-lookup"><span data-stu-id="fcca5-148">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="fcca5-149">status</span><span class="sxs-lookup"><span data-stu-id="fcca5-149">status</span></span>|<span data-ttu-id="fcca5-150">String</span><span class="sxs-lookup"><span data-stu-id="fcca5-150">String</span></span>|<span data-ttu-id="fcca5-151">O estado do ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="fcca5-151">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="fcca5-152">O estado inicial após a criação **é InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="fcca5-152">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="fcca5-153">As transições de estados possíveis **são de InDevelopment** **para Disponível** e **Disponível** **para Preterido**.</span><span class="sxs-lookup"><span data-stu-id="fcca5-153">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="fcca5-154">targetTypes</span><span class="sxs-lookup"><span data-stu-id="fcca5-154">targetTypes</span></span>|<span data-ttu-id="fcca5-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fcca5-155">String collection</span></span>|<span data-ttu-id="fcca5-156">Conjunto de tipos Graph microsoft (que podem dar suporte a extensões) aos quais a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="fcca5-156">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="fcca5-157">Somente alterações aditiva são permitidas.</span><span class="sxs-lookup"><span data-stu-id="fcca5-157">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="fcca5-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcca5-158">Response</span></span>

<span data-ttu-id="fcca5-159">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fcca5-159">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fcca5-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcca5-160">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fcca5-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcca5-161">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="fcca5-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcca5-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
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
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="fcca5-163">C#</span><span class="sxs-lookup"><span data-stu-id="fcca5-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcca5-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcca5-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcca5-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcca5-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcca5-166">Java</span><span class="sxs-lookup"><span data-stu-id="fcca5-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fcca5-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcca5-167">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="fcca5-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="fcca5-168">See also</span></span>

- [<span data-ttu-id="fcca5-169">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="fcca5-169">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fcca5-170">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="fcca5-170">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


