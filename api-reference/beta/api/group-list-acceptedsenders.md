---
title: Listar acceptedSenders
description: Obter uma lista de usuários ou grupos que estão na lista acceptedSenders desse grupo.
author: dkershaw10
ms.openlocfilehash: 8cd753dbdeea78e18e08a75ed4588ff67c225f09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361814"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="010ed-103">Listar acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="010ed-103">List acceptedSenders</span></span>

> <span data-ttu-id="010ed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="010ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="010ed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="010ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="010ed-106">Obter uma lista de usuários ou grupos que estão na lista acceptedSenders desse grupo.</span><span class="sxs-lookup"><span data-stu-id="010ed-106">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="010ed-p102">Os usuários na lista de remetentes aceitos podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="010ed-p102">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="010ed-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="010ed-109">Permissions</span></span>
<span data-ttu-id="010ed-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="010ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="010ed-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="010ed-112">Permission type</span></span>      | <span data-ttu-id="010ed-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="010ed-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="010ed-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="010ed-114">Delegated (work or school account)</span></span> | <span data-ttu-id="010ed-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="010ed-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="010ed-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="010ed-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="010ed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="010ed-117">Not supported.</span></span>    |
|<span data-ttu-id="010ed-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="010ed-118">Application</span></span> | <span data-ttu-id="010ed-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="010ed-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="010ed-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="010ed-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="010ed-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="010ed-121">Optional query parameters</span></span>
<span data-ttu-id="010ed-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="010ed-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="010ed-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="010ed-123">Request headers</span></span>
| <span data-ttu-id="010ed-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="010ed-124">Header</span></span>       | <span data-ttu-id="010ed-125">Valor</span><span class="sxs-lookup"><span data-stu-id="010ed-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="010ed-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="010ed-126">Authorization</span></span>  | <span data-ttu-id="010ed-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="010ed-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="010ed-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="010ed-129">Request body</span></span>
<span data-ttu-id="010ed-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="010ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="010ed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="010ed-131">Response</span></span>
<span data-ttu-id="010ed-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="010ed-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="010ed-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="010ed-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="010ed-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="010ed-134">Request</span></span>
<span data-ttu-id="010ed-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="010ed-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="010ed-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="010ed-136">Response</span></span>
<span data-ttu-id="010ed-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="010ed-137">The following is an example of the response.</span></span>
><span data-ttu-id="010ed-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="010ed-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="010ed-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="010ed-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->