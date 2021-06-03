---
title: Atualizar educationAssignmentResource
description: 'Atualize as propriedades do recurso associado a uma atribuição. Somente professores em uma classe podem alterar objetos de recurso de atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5dae821a6dc22aa108bceee44c4958e3deb7f129
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732998"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="048e2-104">Atualizar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="048e2-104">Update educationAssignmentResource</span></span>

<span data-ttu-id="048e2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="048e2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="048e2-106">Atualize as propriedades do recurso associado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="048e2-106">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="048e2-107">Somente professores em uma classe podem alterar objetos de recurso de atribuição.</span><span class="sxs-lookup"><span data-stu-id="048e2-107">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="048e2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="048e2-108">Permissions</span></span>
<span data-ttu-id="048e2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="048e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="048e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="048e2-111">Permission type</span></span>      | <span data-ttu-id="048e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="048e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="048e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="048e2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="048e2-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="048e2-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="048e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="048e2-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="048e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="048e2-116">Not supported.</span></span>  |
|<span data-ttu-id="048e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="048e2-117">Application</span></span> | <span data-ttu-id="048e2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="048e2-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="048e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="048e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="048e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="048e2-120">Request headers</span></span>
| <span data-ttu-id="048e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="048e2-121">Header</span></span>       | <span data-ttu-id="048e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="048e2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="048e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="048e2-123">Authorization</span></span>  | <span data-ttu-id="048e2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="048e2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="048e2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="048e2-126">Content-Type</span></span>  | <span data-ttu-id="048e2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="048e2-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="048e2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="048e2-128">Request body</span></span>
<span data-ttu-id="048e2-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="048e2-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="048e2-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="048e2-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="048e2-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="048e2-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="048e2-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="048e2-132">Property</span></span>     | <span data-ttu-id="048e2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="048e2-133">Type</span></span>   |<span data-ttu-id="048e2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="048e2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="048e2-135">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="048e2-135">distributeForStudentWork</span></span>|<span data-ttu-id="048e2-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="048e2-136">Boolean</span></span>| <span data-ttu-id="048e2-137">Indica se esse recurso deve ser copiado para o objeto de recurso de cada aluno quando a atribuição for publicada.</span><span class="sxs-lookup"><span data-stu-id="048e2-137">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="048e2-138">recurso</span><span class="sxs-lookup"><span data-stu-id="048e2-138">resource</span></span>|<span data-ttu-id="048e2-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="048e2-139">educationResource</span></span>| <span data-ttu-id="048e2-140">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="048e2-140">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="048e2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="048e2-141">Response</span></span>
<span data-ttu-id="048e2-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="048e2-142">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="048e2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="048e2-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="048e2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="048e2-144">Request</span></span>
<span data-ttu-id="048e2-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="048e2-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="048e2-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="048e2-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="048e2-147">C#</span><span class="sxs-lookup"><span data-stu-id="048e2-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="048e2-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="048e2-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="048e2-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="048e2-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="048e2-150">Java</span><span class="sxs-lookup"><span data-stu-id="048e2-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="048e2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="048e2-151">Response</span></span>
<span data-ttu-id="048e2-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="048e2-152">The following is an example of the response.</span></span> 

><span data-ttu-id="048e2-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="048e2-153">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

{
  "distributeForStudentWork": false,
  "resource": {
      "@odata.type": "#microsoft.graph.educationLinkResource",
      "displayName": "Microsoft Homepage",
      "createdDateTime": "2017-10-21T07:52:45.5675913Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "link": "https://www.microsoft.com"
  },
  "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


