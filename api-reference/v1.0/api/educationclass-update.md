---
title: Atualizar educationClass
description: Atualize as propriedades de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5340a05df5068942c2f895c9858e2f5cd280e24a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231959"
---
# <a name="update-educationclass"></a><span data-ttu-id="a09d9-103">Atualizar educationClass</span><span class="sxs-lookup"><span data-stu-id="a09d9-103">Update educationClass</span></span>

<span data-ttu-id="a09d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a09d9-105">Atualize as propriedades de um [objeto educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="a09d9-105">Update the properties of an [educationClass](../resources/educationclass.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a09d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a09d9-106">Permissions</span></span>
<span data-ttu-id="a09d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a09d9-109">Permission type</span></span>      | <span data-ttu-id="a09d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a09d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a09d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a09d9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a09d9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a09d9-112">Not supported.</span></span>  |
|<span data-ttu-id="a09d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a09d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a09d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a09d9-114">Not supported.</span></span>   |
|<span data-ttu-id="a09d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a09d9-115">Application</span></span> | <span data-ttu-id="a09d9-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09d9-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a09d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a09d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a09d9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a09d9-118">Request headers</span></span>
| <span data-ttu-id="a09d9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a09d9-119">Header</span></span>       | <span data-ttu-id="a09d9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a09d9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a09d9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a09d9-121">Authorization</span></span>  | <span data-ttu-id="a09d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a09d9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a09d9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a09d9-124">Content-Type</span></span>  | <span data-ttu-id="a09d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a09d9-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a09d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a09d9-126">Request body</span></span>
<span data-ttu-id="a09d9-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a09d9-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a09d9-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a09d9-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a09d9-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a09d9-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a09d9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a09d9-130">Property</span></span>             | <span data-ttu-id="a09d9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a09d9-131">Type</span></span>                                               | <span data-ttu-id="a09d9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a09d9-132">Description</span></span>                                                        |
| :------------------- | :------------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="a09d9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a09d9-133">displayName</span></span>          | <span data-ttu-id="a09d9-134">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-134">String</span></span>                                             | <span data-ttu-id="a09d9-135">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="a09d9-135">Name of the class.</span></span>                                                 |
| <span data-ttu-id="a09d9-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a09d9-136">mailNickname</span></span>         | <span data-ttu-id="a09d9-137">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-137">String</span></span>                                             | <span data-ttu-id="a09d9-138">Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="a09d9-138">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="a09d9-139">descrição</span><span class="sxs-lookup"><span data-stu-id="a09d9-139">description</span></span>          | <span data-ttu-id="a09d9-140">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-140">String</span></span>                                             | <span data-ttu-id="a09d9-141">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="a09d9-141">Description of the class.</span></span>                                          |
| <span data-ttu-id="a09d9-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="a09d9-142">createdBy</span></span>            | [<span data-ttu-id="a09d9-143">identitySet</span><span class="sxs-lookup"><span data-stu-id="a09d9-143">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="a09d9-144">Entidade que criou a aula</span><span class="sxs-lookup"><span data-stu-id="a09d9-144">Entity who created the class</span></span>                                       |
| <span data-ttu-id="a09d9-145">classCode</span><span class="sxs-lookup"><span data-stu-id="a09d9-145">classCode</span></span>            | <span data-ttu-id="a09d9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a09d9-146">String</span></span>                                             | <span data-ttu-id="a09d9-147">Código de aula usada pela escola para identificar a aula.</span><span class="sxs-lookup"><span data-stu-id="a09d9-147">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="a09d9-148">externalId</span><span class="sxs-lookup"><span data-stu-id="a09d9-148">externalId</span></span>           | <span data-ttu-id="a09d9-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a09d9-149">String</span></span>                                             | <span data-ttu-id="a09d9-150">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="a09d9-150">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="a09d9-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="a09d9-151">externalSource</span></span>       | <span data-ttu-id="a09d9-152">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="a09d9-152">educationExternalSource</span></span>                            | <span data-ttu-id="a09d9-153">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="a09d9-153">How this class was created.</span></span> <span data-ttu-id="a09d9-154">Os valores possíveis são: `sis` , `manual`</span><span class="sxs-lookup"><span data-stu-id="a09d9-154">Possible values are: `sis`, `manual`</span></span>   |
| <span data-ttu-id="a09d9-155">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="a09d9-155">externalSourceDetail</span></span> | <span data-ttu-id="a09d9-156">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-156">String</span></span>                                             | <span data-ttu-id="a09d9-157">O nome da fonte externa de onde esses recursos foram gerados.</span><span class="sxs-lookup"><span data-stu-id="a09d9-157">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="a09d9-158">grade</span><span class="sxs-lookup"><span data-stu-id="a09d9-158">grade</span></span>                | <span data-ttu-id="a09d9-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a09d9-159">String</span></span>                                             | <span data-ttu-id="a09d9-160">Nível de nota da classe.</span><span class="sxs-lookup"><span data-stu-id="a09d9-160">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="a09d9-161">term</span><span class="sxs-lookup"><span data-stu-id="a09d9-161">term</span></span>                 | [<span data-ttu-id="a09d9-162">educationTerm</span><span class="sxs-lookup"><span data-stu-id="a09d9-162">educationTerm</span></span>](../resources/educationterm.md)     | <span data-ttu-id="a09d9-163">Termos dessa aula.</span><span class="sxs-lookup"><span data-stu-id="a09d9-163">Term for this class.</span></span>                                               |

## <a name="response"></a><span data-ttu-id="a09d9-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09d9-164">Response</span></span>
<span data-ttu-id="a09d9-165">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a09d9-165">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a09d9-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a09d9-166">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a09d9-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a09d9-167">Request</span></span>
<span data-ttu-id="a09d9-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a09d9-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a09d9-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="a09d9-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a09d9-170">C#</span><span class="sxs-lookup"><span data-stu-id="a09d9-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a09d9-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a09d9-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a09d9-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a09d9-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a09d9-173">Java</span><span class="sxs-lookup"><span data-stu-id="a09d9-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a09d9-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09d9-174">Response</span></span>
<span data-ttu-id="a09d9-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a09d9-175">The following is an example of the response.</span></span> 

><span data-ttu-id="a09d9-176">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a09d9-176">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
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
