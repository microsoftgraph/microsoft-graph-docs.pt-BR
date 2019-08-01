---
title: Atualizar propriedades educationclass
description: Atualize as propriedades de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7a3351e3088bce1930a3e3d04341e9b1cacd5dd9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015226"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="b703a-103">Atualizar propriedades educationclass</span><span class="sxs-lookup"><span data-stu-id="b703a-103">Update educationclass properties</span></span>

<span data-ttu-id="b703a-104">Atualize as propriedades de uma aula.</span><span class="sxs-lookup"><span data-stu-id="b703a-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="b703a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b703a-105">Permissions</span></span>
<span data-ttu-id="b703a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b703a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b703a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b703a-108">Permission type</span></span>      | <span data-ttu-id="b703a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b703a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b703a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b703a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b703a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b703a-111">Not supported.</span></span>  |
|<span data-ttu-id="b703a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b703a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b703a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b703a-113">Not supported.</span></span>   |
|<span data-ttu-id="b703a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b703a-114">Application</span></span> | <span data-ttu-id="b703a-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b703a-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b703a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b703a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b703a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b703a-117">Request headers</span></span>
| <span data-ttu-id="b703a-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b703a-118">Header</span></span>       | <span data-ttu-id="b703a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="b703a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b703a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b703a-120">Authorization</span></span>  | <span data-ttu-id="b703a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b703a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b703a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b703a-123">Content-Type</span></span>  | <span data-ttu-id="b703a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b703a-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b703a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b703a-125">Request body</span></span>
<span data-ttu-id="b703a-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b703a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b703a-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b703a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b703a-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b703a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b703a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b703a-129">Property</span></span>     | <span data-ttu-id="b703a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b703a-130">Type</span></span>   |<span data-ttu-id="b703a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b703a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b703a-132">description</span><span class="sxs-lookup"><span data-stu-id="b703a-132">description</span></span>|<span data-ttu-id="b703a-133">String</span><span class="sxs-lookup"><span data-stu-id="b703a-133">String</span></span>| <span data-ttu-id="b703a-134">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="b703a-134">Description of the class.</span></span>|
|<span data-ttu-id="b703a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b703a-135">displayName</span></span>|<span data-ttu-id="b703a-136">String</span><span class="sxs-lookup"><span data-stu-id="b703a-136">String</span></span>| <span data-ttu-id="b703a-137">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="b703a-137">Name of the class.</span></span>|
|<span data-ttu-id="b703a-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b703a-138">mailNickname</span></span>|<span data-ttu-id="b703a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b703a-139">String</span></span>| <span data-ttu-id="b703a-140">Alias de email para envio de email a todos os usuários, se esse recurso estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="b703a-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="b703a-141">|classCode|Cadeia de caracteres| Código de aula usado pela escola.| |externalId|Cadeia de caracteres| ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="b703a-141">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="b703a-142">| |externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.| |externalSource|cadeia de caracteres| Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="b703a-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="b703a-143">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`. |</span><span class="sxs-lookup"><span data-stu-id="b703a-143">The possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="b703a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b703a-144">Response</span></span>
<span data-ttu-id="b703a-145">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b703a-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b703a-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b703a-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b703a-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b703a-147">Request</span></span>
<span data-ttu-id="b703a-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b703a-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b703a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b703a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b703a-150">C#</span><span class="sxs-lookup"><span data-stu-id="b703a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b703a-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="b703a-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b703a-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b703a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b703a-153">Java</span><span class="sxs-lookup"><span data-stu-id="b703a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b703a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b703a-154">Response</span></span>
<span data-ttu-id="b703a-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b703a-155">The following is an example of the response.</span></span> 

><span data-ttu-id="b703a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b703a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
