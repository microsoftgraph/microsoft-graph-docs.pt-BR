---
title: Atualizar propriedades educationclass
description: Atualize as propriedades de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 425d2072e13dbf00d8fc2e81b94cf7da58df8c57
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043718"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="dd907-103">Atualizar propriedades educationclass</span><span class="sxs-lookup"><span data-stu-id="dd907-103">Update educationclass properties</span></span>

<span data-ttu-id="dd907-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd907-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd907-105">Atualize as propriedades de uma aula.</span><span class="sxs-lookup"><span data-stu-id="dd907-105">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd907-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd907-106">Permissions</span></span>
<span data-ttu-id="dd907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd907-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd907-109">Permission type</span></span>      | <span data-ttu-id="dd907-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd907-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd907-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd907-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="dd907-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd907-112">Not supported.</span></span>  |
|<span data-ttu-id="dd907-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd907-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd907-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd907-114">Not supported.</span></span>   |
|<span data-ttu-id="dd907-115">Application</span><span class="sxs-lookup"><span data-stu-id="dd907-115">Application</span></span> | <span data-ttu-id="dd907-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd907-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd907-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd907-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd907-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd907-118">Request headers</span></span>
| <span data-ttu-id="dd907-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd907-119">Header</span></span>       | <span data-ttu-id="dd907-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dd907-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd907-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd907-121">Authorization</span></span>  | <span data-ttu-id="dd907-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd907-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dd907-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd907-124">Content-Type</span></span>  | <span data-ttu-id="dd907-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd907-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd907-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd907-126">Request body</span></span>
<span data-ttu-id="dd907-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="dd907-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dd907-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="dd907-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dd907-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="dd907-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd907-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd907-130">Property</span></span>     | <span data-ttu-id="dd907-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd907-131">Type</span></span>   |<span data-ttu-id="dd907-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd907-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd907-133">description</span><span class="sxs-lookup"><span data-stu-id="dd907-133">description</span></span>|<span data-ttu-id="dd907-134">String</span><span class="sxs-lookup"><span data-stu-id="dd907-134">String</span></span>| <span data-ttu-id="dd907-135">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="dd907-135">Description of the class.</span></span>|
|<span data-ttu-id="dd907-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dd907-136">displayName</span></span>|<span data-ttu-id="dd907-137">String</span><span class="sxs-lookup"><span data-stu-id="dd907-137">String</span></span>| <span data-ttu-id="dd907-138">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="dd907-138">Name of the class.</span></span>|
|<span data-ttu-id="dd907-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="dd907-139">mailNickname</span></span>|<span data-ttu-id="dd907-140">String</span><span class="sxs-lookup"><span data-stu-id="dd907-140">String</span></span>| <span data-ttu-id="dd907-141">Alias de email para envio de email a todos os usuários, se esse recurso estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="dd907-141">Email alias for sending email to all users if that feature is enabled.</span></span> |
|<span data-ttu-id="dd907-142">classCode</span><span class="sxs-lookup"><span data-stu-id="dd907-142">classCode</span></span>|<span data-ttu-id="dd907-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd907-143">String</span></span>| <span data-ttu-id="dd907-144">Código de classe usado pela escola.</span><span class="sxs-lookup"><span data-stu-id="dd907-144">Class code used by the school.</span></span>|
|<span data-ttu-id="dd907-145">externalId</span><span class="sxs-lookup"><span data-stu-id="dd907-145">externalId</span></span>|<span data-ttu-id="dd907-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd907-146">String</span></span>| <span data-ttu-id="dd907-147">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="dd907-147">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="dd907-148">externalName</span><span class="sxs-lookup"><span data-stu-id="dd907-148">externalName</span></span>|<span data-ttu-id="dd907-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd907-149">String</span></span>|<span data-ttu-id="dd907-150">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="dd907-150">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="dd907-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="dd907-151">externalSource</span></span>|<span data-ttu-id="dd907-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd907-152">string</span></span>| <span data-ttu-id="dd907-153">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="dd907-153">How this class was created.</span></span> <span data-ttu-id="dd907-154">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="dd907-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|

## <a name="response"></a><span data-ttu-id="dd907-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd907-155">Response</span></span>
<span data-ttu-id="dd907-156">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd907-156">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd907-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd907-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd907-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd907-158">Request</span></span>
<span data-ttu-id="dd907-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd907-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd907-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd907-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="c"></a>[<span data-ttu-id="dd907-161">C#</span><span class="sxs-lookup"><span data-stu-id="dd907-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd907-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd907-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd907-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd907-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd907-164">Java</span><span class="sxs-lookup"><span data-stu-id="dd907-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd907-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd907-165">Response</span></span>
<span data-ttu-id="dd907-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd907-166">The following is an example of the response.</span></span>

><span data-ttu-id="dd907-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dd907-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


