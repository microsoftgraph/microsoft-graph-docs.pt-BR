---
title: Criar tokenLifetimePolicy
description: Criar um novo tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f52dd8ebfd4273b7d32f3c64b22d163b83b4fa9b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229532"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="eef33-103">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="eef33-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="eef33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef33-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="eef33-105">Criar um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="eef33-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eef33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eef33-106">Permissions</span></span>

<span data-ttu-id="eef33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eef33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eef33-109">Permission type</span></span>                        | <span data-ttu-id="eef33-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eef33-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eef33-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eef33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eef33-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="eef33-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="eef33-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eef33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eef33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eef33-114">Not supported.</span></span> |
| <span data-ttu-id="eef33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eef33-115">Application</span></span>                            | <span data-ttu-id="eef33-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="eef33-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="eef33-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eef33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="eef33-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eef33-118">Request headers</span></span>

| <span data-ttu-id="eef33-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eef33-119">Name</span></span>          | <span data-ttu-id="eef33-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef33-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eef33-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eef33-121">Authorization</span></span> | <span data-ttu-id="eef33-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eef33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eef33-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="eef33-124">Content-type</span></span> | <span data-ttu-id="eef33-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eef33-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eef33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eef33-127">Request body</span></span>

<span data-ttu-id="eef33-128">No corpo da solicitação, forneça uma representação JSON do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="eef33-128">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eef33-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef33-129">Response</span></span>

<span data-ttu-id="eef33-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eef33-130">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eef33-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eef33-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eef33-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eef33-132">Request</span></span>

<span data-ttu-id="eef33-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eef33-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="eef33-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef33-134">Response</span></span>

<span data-ttu-id="eef33-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eef33-135">The following is an example of the response.</span></span>

> <span data-ttu-id="eef33-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eef33-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
