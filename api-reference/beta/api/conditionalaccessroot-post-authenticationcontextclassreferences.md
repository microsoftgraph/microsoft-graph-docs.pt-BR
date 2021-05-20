---
title: Criar authenticationContextClassReference
description: Crie uma nova autenticaçãoContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8ad536988d73e8550ec4561f0ca6ead77c40d256
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547305"
---
# <a name="create-authenticationcontextclassreference"></a><span data-ttu-id="c2c88-103">Criar authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="c2c88-103">Create authenticationContextClassReference</span></span>

<span data-ttu-id="c2c88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2c88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2c88-105">Criar uma nova [autenticaçãoContextClassReference](../resources/authenticationContextClassReference.md).</span><span class="sxs-lookup"><span data-stu-id="c2c88-105">Create a new [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2c88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2c88-106">Permissions</span></span>

<span data-ttu-id="c2c88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2c88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2c88-109">Permission type</span></span>                        | <span data-ttu-id="c2c88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2c88-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="c2c88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2c88-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2c88-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="c2c88-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="c2c88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2c88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2c88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2c88-114">Not supported.</span></span> |
|<span data-ttu-id="c2c88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2c88-115">Application</span></span>                            | <span data-ttu-id="c2c88-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="c2c88-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="c2c88-117">Essa API tem um [problema conhecido relacionado](/graph/known-issues#permissions) a permissões.</span><span class="sxs-lookup"><span data-stu-id="c2c88-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2c88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2c88-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a><span data-ttu-id="c2c88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c88-119">Request headers</span></span>

| <span data-ttu-id="c2c88-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c2c88-120">Name</span></span>          | <span data-ttu-id="c2c88-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2c88-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="c2c88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2c88-122">Authorization</span></span> | <span data-ttu-id="c2c88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2c88-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c2c88-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2c88-125">Content-Type</span></span>  | <span data-ttu-id="c2c88-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2c88-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2c88-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c88-128">Request body</span></span>

<span data-ttu-id="c2c88-129">No corpo da solicitação, fornece uma representação JSON de um [objeto authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="c2c88-129">In the request body, supply a JSON representation of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2c88-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2c88-130">Response</span></span>

<span data-ttu-id="c2c88-131">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto authenticationContextClassReference](../resources/authenticationcontextclassreference.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2c88-131">If successful, this method returns a `201 Created` response code and a new [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2c88-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c2c88-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2c88-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c88-133">Request</span></span>
<span data-ttu-id="c2c88-134">O exemplo a seguir mostra a criação de uma nova authenticationcontextclassreference que está disponível para aplicativos usarem.</span><span class="sxs-lookup"><span data-stu-id="c2c88-134">The following example shows creating a new authenticationcontextclassreference that is available for apps to use.</span></span>



<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```



#### <a name="response"></a><span data-ttu-id="c2c88-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2c88-135">Response</span></span>

<span data-ttu-id="c2c88-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2c88-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
