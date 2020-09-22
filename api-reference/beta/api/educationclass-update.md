---
title: Atualizar propriedades educationclass
description: Atualize as propriedades de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8b339ceb2f48695692a7258c59944df74d9bd186
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007529"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="2107f-103">Atualizar propriedades educationclass</span><span class="sxs-lookup"><span data-stu-id="2107f-103">Update educationclass properties</span></span>

<span data-ttu-id="2107f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2107f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2107f-105">Atualize as propriedades de uma aula.</span><span class="sxs-lookup"><span data-stu-id="2107f-105">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="2107f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2107f-106">Permissions</span></span>
<span data-ttu-id="2107f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2107f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2107f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2107f-109">Permission type</span></span>      | <span data-ttu-id="2107f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2107f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2107f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2107f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2107f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2107f-112">Not supported.</span></span>  |
|<span data-ttu-id="2107f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2107f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2107f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2107f-114">Not supported.</span></span>   |
|<span data-ttu-id="2107f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2107f-115">Application</span></span> | <span data-ttu-id="2107f-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2107f-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2107f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2107f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2107f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2107f-118">Request headers</span></span>
| <span data-ttu-id="2107f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2107f-119">Header</span></span>       | <span data-ttu-id="2107f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2107f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2107f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2107f-121">Authorization</span></span>  | <span data-ttu-id="2107f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2107f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2107f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2107f-124">Content-Type</span></span>  | <span data-ttu-id="2107f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2107f-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2107f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2107f-126">Request body</span></span>
<span data-ttu-id="2107f-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2107f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2107f-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2107f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2107f-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2107f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2107f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2107f-130">Property</span></span>     | <span data-ttu-id="2107f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2107f-131">Type</span></span>   |<span data-ttu-id="2107f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2107f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2107f-133">description</span><span class="sxs-lookup"><span data-stu-id="2107f-133">description</span></span>|<span data-ttu-id="2107f-134">String</span><span class="sxs-lookup"><span data-stu-id="2107f-134">String</span></span>| <span data-ttu-id="2107f-135">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="2107f-135">Description of the class.</span></span>|
|<span data-ttu-id="2107f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2107f-136">displayName</span></span>|<span data-ttu-id="2107f-137">String</span><span class="sxs-lookup"><span data-stu-id="2107f-137">String</span></span>| <span data-ttu-id="2107f-138">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="2107f-138">Name of the class.</span></span>|
|<span data-ttu-id="2107f-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2107f-139">mailNickname</span></span>|<span data-ttu-id="2107f-140">String</span><span class="sxs-lookup"><span data-stu-id="2107f-140">String</span></span>| <span data-ttu-id="2107f-141">Alias de email para envio de email a todos os usuários, se esse recurso estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="2107f-141">Email alias for sending email to all users if that feature is enabled.</span></span> |
|<span data-ttu-id="2107f-142">classCode</span><span class="sxs-lookup"><span data-stu-id="2107f-142">classCode</span></span>|<span data-ttu-id="2107f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2107f-143">String</span></span>| <span data-ttu-id="2107f-144">Código de classe usado pela escola.</span><span class="sxs-lookup"><span data-stu-id="2107f-144">Class code used by the school.</span></span>|
|<span data-ttu-id="2107f-145">externalId</span><span class="sxs-lookup"><span data-stu-id="2107f-145">externalId</span></span>|<span data-ttu-id="2107f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2107f-146">String</span></span>| <span data-ttu-id="2107f-147">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2107f-147">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="2107f-148">externalName</span><span class="sxs-lookup"><span data-stu-id="2107f-148">externalName</span></span>|<span data-ttu-id="2107f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2107f-149">String</span></span>|<span data-ttu-id="2107f-150">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2107f-150">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="2107f-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="2107f-151">externalSource</span></span>|<span data-ttu-id="2107f-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2107f-152">string</span></span>| <span data-ttu-id="2107f-153">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="2107f-153">How this class was created.</span></span> <span data-ttu-id="2107f-154">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2107f-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|

## <a name="response"></a><span data-ttu-id="2107f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="2107f-155">Response</span></span>
<span data-ttu-id="2107f-156">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2107f-156">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2107f-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2107f-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2107f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2107f-158">Request</span></span>
<span data-ttu-id="2107f-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2107f-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2107f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="2107f-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2107f-161">C#</span><span class="sxs-lookup"><span data-stu-id="2107f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2107f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2107f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2107f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2107f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2107f-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="2107f-164">Response</span></span>
<span data-ttu-id="2107f-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2107f-165">The following is an example of the response.</span></span>

><span data-ttu-id="2107f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2107f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


