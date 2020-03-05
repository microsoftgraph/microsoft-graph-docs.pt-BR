---
title: Obter política
description: Recupere as propriedades de uma política.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d9813151c2dde323ed685592ad6c00979d9c3f01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455535"
---
# <a name="get-policy"></a><span data-ttu-id="24144-103">Obter política</span><span class="sxs-lookup"><span data-stu-id="24144-103">Get Policy</span></span>

<span data-ttu-id="24144-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="24144-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24144-105">Recupere as propriedades de uma [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="24144-105">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24144-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24144-106">Permissions</span></span>
<span data-ttu-id="24144-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24144-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24144-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24144-109">Permission type</span></span>      | <span data-ttu-id="24144-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24144-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24144-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24144-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24144-112">Policy. Read. All, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="24144-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24144-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24144-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24144-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24144-114">Not supported.</span></span>    |
|<span data-ttu-id="24144-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24144-115">Application</span></span> | <span data-ttu-id="24144-116">Policy. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="24144-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24144-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24144-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="24144-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24144-118">Request headers</span></span>
| <span data-ttu-id="24144-119">Nome</span><span class="sxs-lookup"><span data-stu-id="24144-119">Name</span></span>       | <span data-ttu-id="24144-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="24144-120">Type</span></span> | <span data-ttu-id="24144-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="24144-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24144-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24144-122">Authorization</span></span>  | <span data-ttu-id="24144-123">string</span><span class="sxs-lookup"><span data-stu-id="24144-123">string</span></span>  | <span data-ttu-id="24144-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24144-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24144-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24144-126">Request body</span></span>
<span data-ttu-id="24144-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24144-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24144-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="24144-128">Response</span></span>

<span data-ttu-id="24144-129">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24144-129">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="24144-130">Se unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="24144-130">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="24144-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24144-131">Example</span></span>
<span data-ttu-id="24144-132">O exemplo a seguir recupera uma política específica.</span><span class="sxs-lookup"><span data-stu-id="24144-132">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="24144-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24144-133">Request</span></span>
<span data-ttu-id="24144-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24144-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="24144-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="24144-135">Response</span></span>
<span data-ttu-id="24144-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24144-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
