---
title: 'servicePrincipalName: getMemberObjects'
description: Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.  Essa verificação é transitiva.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: afa2e48691ba421fad8ffc1c2f5ae630591295d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453453"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="4761b-104">servicePrincipalName: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4761b-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="4761b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4761b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4761b-106">Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="4761b-106">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="4761b-107">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="4761b-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4761b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4761b-108">Permissions</span></span>
<span data-ttu-id="4761b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4761b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4761b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4761b-111">Permission type</span></span>      | <span data-ttu-id="4761b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4761b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4761b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4761b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4761b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4761b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4761b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4761b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4761b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4761b-116">Not supported.</span></span>    |
|<span data-ttu-id="4761b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4761b-117">Application</span></span> | <span data-ttu-id="4761b-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4761b-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4761b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4761b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="4761b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4761b-120">Request headers</span></span>
| <span data-ttu-id="4761b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4761b-121">Name</span></span>       | <span data-ttu-id="4761b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="4761b-122">Type</span></span> | <span data-ttu-id="4761b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4761b-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4761b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4761b-124">Authorization</span></span>  | <span data-ttu-id="4761b-125">string</span><span class="sxs-lookup"><span data-stu-id="4761b-125">string</span></span>  | <span data-ttu-id="4761b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4761b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4761b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4761b-128">Request body</span></span>
<span data-ttu-id="4761b-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4761b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4761b-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4761b-130">Parameter</span></span>    | <span data-ttu-id="4761b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4761b-131">Type</span></span>   |<span data-ttu-id="4761b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4761b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4761b-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4761b-133">securityEnabledOnly</span></span>|<span data-ttu-id="4761b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4761b-134">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="4761b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4761b-135">Response</span></span>

<span data-ttu-id="4761b-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4761b-136">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4761b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4761b-137">Example</span></span>
<span data-ttu-id="4761b-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4761b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4761b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4761b-139">Request</span></span>
<span data-ttu-id="4761b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4761b-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4761b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4761b-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4761b-142">C#</span><span class="sxs-lookup"><span data-stu-id="4761b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4761b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4761b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4761b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4761b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4761b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4761b-145">Response</span></span>
<span data-ttu-id="4761b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4761b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
