---
title: 'servicePrincipalName: checkMemberGroups'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
ms.openlocfilehash: e59e4c30793b2c05cb3f050be9acfa31331777cd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453772"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="e82e0-104">servicePrincipalName: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e82e0-104">servicePrincipal: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="e82e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e82e0-105">Permissions</span></span>
<span data-ttu-id="e82e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e82e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e82e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e82e0-108">Permission type</span></span>      | <span data-ttu-id="e82e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e82e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e82e0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e82e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e82e0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e82e0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e82e0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e82e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e82e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e82e0-113">Not supported.</span></span>    |
|<span data-ttu-id="e82e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e82e0-114">Application</span></span> | <span data-ttu-id="e82e0-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e82e0-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e82e0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e82e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e82e0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e82e0-117">Request headers</span></span>
| <span data-ttu-id="e82e0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e82e0-118">Name</span></span>       | <span data-ttu-id="e82e0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82e0-119">Type</span></span> | <span data-ttu-id="e82e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82e0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e82e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e82e0-121">Authorization</span></span>  | <span data-ttu-id="e82e0-122">string</span><span class="sxs-lookup"><span data-stu-id="e82e0-122">string</span></span>  | <span data-ttu-id="e82e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e82e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e82e0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e82e0-125">Request body</span></span>
<span data-ttu-id="e82e0-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e82e0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e82e0-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e82e0-127">Parameter</span></span>    | <span data-ttu-id="e82e0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82e0-128">Type</span></span>   |<span data-ttu-id="e82e0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82e0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e82e0-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="e82e0-130">groupIds</span></span>|<span data-ttu-id="e82e0-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e82e0-131">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="e82e0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e82e0-132">Response</span></span>

<span data-ttu-id="e82e0-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e82e0-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e82e0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e82e0-134">Example</span></span>
<span data-ttu-id="e82e0-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e82e0-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e82e0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e82e0-136">Request</span></span>
<span data-ttu-id="e82e0-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e82e0-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e82e0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e82e0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e82e0-139">C#</span><span class="sxs-lookup"><span data-stu-id="e82e0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e82e0-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e82e0-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e82e0-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e82e0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e82e0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e82e0-142">Response</span></span>
<span data-ttu-id="e82e0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e82e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
