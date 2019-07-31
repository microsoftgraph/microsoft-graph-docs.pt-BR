---
title: 'servicePrincipalName: getMemberObjects'
description: Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.  Essa verificação é transitiva.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 440bbf9a51f0b1b7b13fc42397307e47ad0cff75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991468"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="95c67-104">servicePrincipalName: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="95c67-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c67-105">Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="95c67-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="95c67-106">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="95c67-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="95c67-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="95c67-107">Permissions</span></span>
<span data-ttu-id="95c67-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c67-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95c67-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95c67-110">Permission type</span></span>      | <span data-ttu-id="95c67-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95c67-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95c67-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95c67-112">Delegated (work or school account)</span></span> | <span data-ttu-id="95c67-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95c67-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95c67-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95c67-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95c67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c67-115">Not supported.</span></span>    |
|<span data-ttu-id="95c67-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95c67-116">Application</span></span> | <span data-ttu-id="95c67-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95c67-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95c67-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95c67-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="95c67-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95c67-119">Request headers</span></span>
| <span data-ttu-id="95c67-120">Nome</span><span class="sxs-lookup"><span data-stu-id="95c67-120">Name</span></span>       | <span data-ttu-id="95c67-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="95c67-121">Type</span></span> | <span data-ttu-id="95c67-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c67-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95c67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95c67-123">Authorization</span></span>  | <span data-ttu-id="95c67-124">string</span><span class="sxs-lookup"><span data-stu-id="95c67-124">string</span></span>  | <span data-ttu-id="95c67-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95c67-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95c67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95c67-127">Request body</span></span>
<span data-ttu-id="95c67-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95c67-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95c67-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="95c67-129">Parameter</span></span>    | <span data-ttu-id="95c67-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="95c67-130">Type</span></span>   |<span data-ttu-id="95c67-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c67-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95c67-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="95c67-132">securityEnabledOnly</span></span>|<span data-ttu-id="95c67-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="95c67-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="95c67-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c67-134">Response</span></span>

<span data-ttu-id="95c67-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c67-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95c67-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95c67-136">Example</span></span>
<span data-ttu-id="95c67-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="95c67-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95c67-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c67-138">Request</span></span>
<span data-ttu-id="95c67-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95c67-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95c67-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="95c67-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95c67-141">C#</span><span class="sxs-lookup"><span data-stu-id="95c67-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95c67-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="95c67-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95c67-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="95c67-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="95c67-144">Java</span><span class="sxs-lookup"><span data-stu-id="95c67-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="95c67-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c67-145">Response</span></span>
<span data-ttu-id="95c67-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95c67-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
