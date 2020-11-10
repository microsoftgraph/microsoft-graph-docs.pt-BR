---
title: Update schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 126d68f60ea412686324880fc206914e4fc588af
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978729"
---
# <a name="update-schemaextension"></a><span data-ttu-id="f4e22-103">Update schemaExtension</span><span class="sxs-lookup"><span data-stu-id="f4e22-103">Update schemaExtension</span></span>

<span data-ttu-id="f4e22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4e22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4e22-105">Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="f4e22-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="f4e22-106">A atualização se aplica a todos os recursos incluídos na propriedade **TargetTypes** da extensão.</span><span class="sxs-lookup"><span data-stu-id="f4e22-106">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="f4e22-107">Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="f4e22-107">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="f4e22-108">Somente o aplicativo que criou uma extensão de esquema (aplicativo proprietário) pode fazer atualizações aditivas para a extensão quando a extensão está no **indesenvolvimento** ou status **disponível** .</span><span class="sxs-lookup"><span data-stu-id="f4e22-108">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="f4e22-109">Isso significa que o aplicativo não pode remover propriedades personalizadas ou tipos de recurso de destino da definição.</span><span class="sxs-lookup"><span data-stu-id="f4e22-109">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="f4e22-110">No entanto, o aplicativo pode alterar a descrição da extensão.</span><span class="sxs-lookup"><span data-stu-id="f4e22-110">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4e22-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4e22-111">Permissions</span></span>

<span data-ttu-id="f4e22-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e22-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f4e22-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4e22-114">Permission type</span></span>      | <span data-ttu-id="f4e22-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4e22-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4e22-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4e22-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f4e22-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4e22-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4e22-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4e22-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4e22-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4e22-119">Not supported.</span></span>    |
|<span data-ttu-id="f4e22-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4e22-120">Application</span></span> | <span data-ttu-id="f4e22-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4e22-121">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="f4e22-122">Adicionalmente para o fluxo delegado, o usuário conectado só pode atualizar schemaExtensions que possuem (onde a propriedade **Owner** do schemaExtension é o `appId` de um aplicativo que o usuário conectado possui).</span><span class="sxs-lookup"><span data-stu-id="f4e22-122">Additionally for the delegated flow, the signed-in user can only update schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="f4e22-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4e22-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f4e22-124">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f4e22-124">Optional request headers</span></span>

| <span data-ttu-id="f4e22-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f4e22-125">Name</span></span>      |<span data-ttu-id="f4e22-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e22-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4e22-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4e22-127">Authorization</span></span>  | <span data-ttu-id="f4e22-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4e22-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4e22-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4e22-130">Content-Type</span></span>   | <span data-ttu-id="f4e22-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f4e22-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4e22-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4e22-132">Request body</span></span>

<span data-ttu-id="f4e22-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f4e22-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f4e22-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4e22-136">Property</span></span>   | <span data-ttu-id="f4e22-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4e22-137">Type</span></span> |<span data-ttu-id="f4e22-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e22-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4e22-139">description</span><span class="sxs-lookup"><span data-stu-id="f4e22-139">description</span></span>|<span data-ttu-id="f4e22-140">String</span><span class="sxs-lookup"><span data-stu-id="f4e22-140">String</span></span>|<span data-ttu-id="f4e22-141">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="f4e22-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="f4e22-142">properties</span><span class="sxs-lookup"><span data-stu-id="f4e22-142">properties</span></span>|<span data-ttu-id="f4e22-143">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f4e22-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="f4e22-144">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="f4e22-144">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="f4e22-145">Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="f4e22-145">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="f4e22-146">status</span><span class="sxs-lookup"><span data-stu-id="f4e22-146">status</span></span>|<span data-ttu-id="f4e22-147">String</span><span class="sxs-lookup"><span data-stu-id="f4e22-147">String</span></span>|<span data-ttu-id="f4e22-148">O estado do ciclo de vida da extensão do esquema.</span><span class="sxs-lookup"><span data-stu-id="f4e22-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="f4e22-149">O estado inicial na criação é o **indevelopment**.</span><span class="sxs-lookup"><span data-stu-id="f4e22-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="f4e22-150">Os possíveis transições de Estados estão de **indevelopment** para **Available** e **disponíveis** para **preteridos**.</span><span class="sxs-lookup"><span data-stu-id="f4e22-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="f4e22-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="f4e22-151">targetTypes</span></span>|<span data-ttu-id="f4e22-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e22-152">String collection</span></span>|<span data-ttu-id="f4e22-153">Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="f4e22-153">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="f4e22-154">Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="f4e22-154">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="f4e22-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4e22-155">Response</span></span>

<span data-ttu-id="f4e22-156">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4e22-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4e22-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4e22-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f4e22-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4e22-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f4e22-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4e22-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f4e22-160">C#</span><span class="sxs-lookup"><span data-stu-id="f4e22-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4e22-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4e22-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4e22-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4e22-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4e22-163">Java</span><span class="sxs-lookup"><span data-stu-id="f4e22-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f4e22-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4e22-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="f4e22-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="f4e22-165">See also</span></span>

- [<span data-ttu-id="f4e22-166">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f4e22-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f4e22-167">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="f4e22-167">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


