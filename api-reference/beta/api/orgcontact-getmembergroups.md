---
title: 'orgContact: getMemberGroups'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8f98e07e77b05958f50d6ab1f00d944e95aa37ff
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657228"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="ee536-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ee536-104">orgContact: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="ee536-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee536-105">Permissions</span></span>
<span data-ttu-id="ee536-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee536-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee536-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee536-108">Permission type</span></span>      | <span data-ttu-id="ee536-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee536-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee536-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee536-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee536-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee536-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee536-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee536-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee536-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee536-113">Not supported.</span></span>    |
|<span data-ttu-id="ee536-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee536-114">Application</span></span> | <span data-ttu-id="ee536-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee536-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee536-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee536-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="ee536-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee536-117">Request headers</span></span>
| <span data-ttu-id="ee536-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ee536-118">Name</span></span>       | <span data-ttu-id="ee536-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee536-119">Type</span></span> | <span data-ttu-id="ee536-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee536-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee536-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee536-121">Authorization</span></span>  | <span data-ttu-id="ee536-122">string</span><span class="sxs-lookup"><span data-stu-id="ee536-122">string</span></span>  | <span data-ttu-id="ee536-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee536-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee536-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee536-125">Request body</span></span>
<span data-ttu-id="ee536-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee536-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ee536-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ee536-127">Parameter</span></span>    | <span data-ttu-id="ee536-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee536-128">Type</span></span>   |<span data-ttu-id="ee536-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee536-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee536-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ee536-130">securityEnabledOnly</span></span>|<span data-ttu-id="ee536-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee536-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="ee536-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee536-132">Response</span></span>

<span data-ttu-id="ee536-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee536-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee536-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee536-134">Example</span></span>
<span data-ttu-id="ee536-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ee536-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee536-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee536-136">Request</span></span>
<span data-ttu-id="ee536-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee536-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="ee536-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee536-138">Response</span></span>
<span data-ttu-id="ee536-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee536-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ee536-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ee536-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ee536-143">C#</span><span class="sxs-lookup"><span data-stu-id="ee536-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/orgcontact_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee536-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee536-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/orgcontact_getmembergroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
