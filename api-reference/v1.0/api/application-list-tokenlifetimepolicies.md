---
title: Lista atribuída tokenLifetimePolicies
description: Listar tokenLifetimePolicies atribuídos a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c26574d4720765c292f0bb606e57a7c07927b03f
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229083"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="b51dc-103">Lista atribuída tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b51dc-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="b51dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b51dc-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b51dc-105">Lista os objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) que são atribuídos a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="b51dc-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b51dc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b51dc-106">Permissions</span></span>

<span data-ttu-id="b51dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b51dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b51dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b51dc-109">Permission type</span></span>                        | <span data-ttu-id="b51dc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b51dc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b51dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b51dc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b51dc-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b51dc-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b51dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b51dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b51dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b51dc-114">Not supported.</span></span> |
| <span data-ttu-id="b51dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b51dc-115">Application</span></span>                            | <span data-ttu-id="b51dc-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b51dc-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b51dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b51dc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b51dc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b51dc-118">Request headers</span></span>

| <span data-ttu-id="b51dc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b51dc-119">Name</span></span>          | <span data-ttu-id="b51dc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b51dc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b51dc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b51dc-121">Authorization</span></span> | <span data-ttu-id="b51dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b51dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b51dc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b51dc-124">Request body</span></span>

<span data-ttu-id="b51dc-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b51dc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b51dc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b51dc-126">Response</span></span>

<span data-ttu-id="b51dc-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b51dc-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b51dc-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b51dc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b51dc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b51dc-129">Request</span></span>

<span data-ttu-id="b51dc-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b51dc-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```

### <a name="response"></a><span data-ttu-id="b51dc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b51dc-131">Response</span></span>

<span data-ttu-id="b51dc-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b51dc-132">The following is an example of the response.</span></span>

> <span data-ttu-id="b51dc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b51dc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
