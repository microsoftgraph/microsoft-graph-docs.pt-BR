---
title: Listar rejectedSenders
description: 'Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo. '
author: dkershaw10
ms.openlocfilehash: aa79ec70982e75349c41ecb551cbf0150b82ad60
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336075"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="779ef-103">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="779ef-103">List rejectedSenders</span></span>

> <span data-ttu-id="779ef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="779ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="779ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="779ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="779ef-106">Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo.</span><span class="sxs-lookup"><span data-stu-id="779ef-106">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="779ef-p102">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="779ef-p102">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="779ef-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="779ef-109">Permissions</span></span>
<span data-ttu-id="779ef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="779ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="779ef-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="779ef-112">Permission type</span></span>      | <span data-ttu-id="779ef-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="779ef-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="779ef-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="779ef-114">Delegated (work or school account)</span></span> | <span data-ttu-id="779ef-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779ef-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="779ef-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="779ef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="779ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="779ef-117">Not supported.</span></span>    |
|<span data-ttu-id="779ef-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="779ef-118">Application</span></span> | <span data-ttu-id="779ef-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="779ef-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="779ef-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="779ef-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="779ef-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="779ef-121">Optional query parameters</span></span>
<span data-ttu-id="779ef-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="779ef-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="779ef-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="779ef-123">Request headers</span></span>
| <span data-ttu-id="779ef-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="779ef-124">Header</span></span>       | <span data-ttu-id="779ef-125">Valor</span><span class="sxs-lookup"><span data-stu-id="779ef-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="779ef-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="779ef-126">Authorization</span></span>  | <span data-ttu-id="779ef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="779ef-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="779ef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="779ef-129">Request body</span></span>
<span data-ttu-id="779ef-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="779ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="779ef-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="779ef-131">Response</span></span>
<span data-ttu-id="779ef-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="779ef-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="779ef-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="779ef-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="779ef-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="779ef-134">Request</span></span>
<span data-ttu-id="779ef-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="779ef-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="779ef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="779ef-136">Response</span></span>
<span data-ttu-id="779ef-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="779ef-137">The following is an example of the response.</span></span>
><span data-ttu-id="779ef-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="779ef-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="779ef-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="779ef-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->