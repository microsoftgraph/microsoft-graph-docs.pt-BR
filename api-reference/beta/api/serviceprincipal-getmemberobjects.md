---
title: 'servicePrincipalName: getMemberObjects'
description: Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.  Essa verificação é transitiva.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 689eb4514207d58cb69a2ea0a32cd89fea93d5b0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219281"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="e5e8d-104">servicePrincipalName: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e5e8d-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="e5e8d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5e8d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5e8d-106">Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-106">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="e5e8d-107">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5e8d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5e8d-108">Permissions</span></span>
<span data-ttu-id="e5e8d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5e8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5e8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5e8d-111">Permission type</span></span>      | <span data-ttu-id="e5e8d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5e8d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5e8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5e8d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e5e8d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5e8d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5e8d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5e8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5e8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-116">Not supported.</span></span>    |
|<span data-ttu-id="e5e8d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5e8d-117">Application</span></span> | <span data-ttu-id="e5e8d-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e8d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5e8d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5e8d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="e5e8d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5e8d-120">Request headers</span></span>
| <span data-ttu-id="e5e8d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e5e8d-121">Name</span></span>       | <span data-ttu-id="e5e8d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5e8d-122">Type</span></span> | <span data-ttu-id="e5e8d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5e8d-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5e8d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5e8d-124">Authorization</span></span>  | <span data-ttu-id="e5e8d-125">string</span><span class="sxs-lookup"><span data-stu-id="e5e8d-125">string</span></span>  | <span data-ttu-id="e5e8d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5e8d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5e8d-128">Request body</span></span>
<span data-ttu-id="e5e8d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5e8d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5e8d-130">Parameter</span></span>    | <span data-ttu-id="e5e8d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5e8d-131">Type</span></span>   |<span data-ttu-id="e5e8d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5e8d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5e8d-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e5e8d-133">securityEnabledOnly</span></span>|<span data-ttu-id="e5e8d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5e8d-134">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="e5e8d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5e8d-135">Response</span></span>

<span data-ttu-id="e5e8d-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-136">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5e8d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5e8d-137">Example</span></span>
<span data-ttu-id="e5e8d-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5e8d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5e8d-139">Request</span></span>
<span data-ttu-id="e5e8d-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5e8d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5e8d-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e5e8d-142">C#</span><span class="sxs-lookup"><span data-stu-id="e5e8d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5e8d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5e8d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5e8d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5e8d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5e8d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5e8d-145">Response</span></span>
<span data-ttu-id="e5e8d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5e8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
