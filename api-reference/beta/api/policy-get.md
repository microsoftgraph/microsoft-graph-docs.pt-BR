---
title: Obter política
description: Recupere as propriedades de uma política.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: d9be2517424156042568de1ee9a5f86c07a889a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450876"
---
# <a name="get-policy"></a><span data-ttu-id="66d78-103">Obter política</span><span class="sxs-lookup"><span data-stu-id="66d78-103">Get Policy</span></span>

<span data-ttu-id="66d78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66d78-105">Recupere as propriedades de uma [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="66d78-105">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66d78-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66d78-106">Permissions</span></span>
<span data-ttu-id="66d78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66d78-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66d78-109">Permission type</span></span>      | <span data-ttu-id="66d78-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66d78-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d78-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66d78-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66d78-112">Policy. Read. All, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="66d78-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66d78-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66d78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d78-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d78-114">Not supported.</span></span>    |
|<span data-ttu-id="66d78-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66d78-115">Application</span></span> | <span data-ttu-id="66d78-116">Policy. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="66d78-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d78-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66d78-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="66d78-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66d78-118">Request headers</span></span>
| <span data-ttu-id="66d78-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66d78-119">Name</span></span>       | <span data-ttu-id="66d78-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d78-120">Type</span></span> | <span data-ttu-id="66d78-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d78-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66d78-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66d78-122">Authorization</span></span>  | <span data-ttu-id="66d78-123">string</span><span class="sxs-lookup"><span data-stu-id="66d78-123">string</span></span>  | <span data-ttu-id="66d78-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66d78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66d78-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66d78-126">Request body</span></span>
<span data-ttu-id="66d78-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66d78-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66d78-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d78-128">Response</span></span>

<span data-ttu-id="66d78-129">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d78-129">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="66d78-130">Se unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="66d78-130">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="66d78-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66d78-131">Example</span></span>
<span data-ttu-id="66d78-132">O exemplo a seguir recupera uma política específica.</span><span class="sxs-lookup"><span data-stu-id="66d78-132">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="66d78-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66d78-133">Request</span></span>
<span data-ttu-id="66d78-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d78-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="66d78-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d78-135">Response</span></span>
<span data-ttu-id="66d78-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66d78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
