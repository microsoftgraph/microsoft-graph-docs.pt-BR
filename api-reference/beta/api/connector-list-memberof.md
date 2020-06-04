---
title: Listar memberOf
description: Recupere o MemberGroup do qual o conector é membro.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 07d68b91d548b990f609d4c4d43424999d68e846
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556079"
---
# <a name="list-memberof"></a><span data-ttu-id="3bc7b-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="3bc7b-103">List memberOf</span></span>

<span data-ttu-id="3bc7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bc7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bc7b-105">Recupere o [MemberGroup do qual o](../resources/connectorgroup.md) [conector](../resources/connector.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-105">Retrieve the [connectorGroup](../resources/connectorgroup.md) the [connector](../resources/connector.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bc7b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bc7b-106">Permissions</span></span>
<span data-ttu-id="3bc7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bc7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bc7b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bc7b-109">Permission type</span></span>      | <span data-ttu-id="3bc7b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bc7b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bc7b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bc7b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3bc7b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bc7b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bc7b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bc7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bc7b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-114">Not supported.</span></span>    |
|<span data-ttu-id="3bc7b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bc7b-115">Application</span></span> | <span data-ttu-id="3bc7b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc7b-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bc7b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bc7b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3bc7b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bc7b-118">Optional query parameters</span></span>
<span data-ttu-id="3bc7b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bc7b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc7b-120">Request headers</span></span>
| <span data-ttu-id="3bc7b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3bc7b-121">Name</span></span>      |<span data-ttu-id="3bc7b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc7b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3bc7b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bc7b-123">Authorization</span></span>  | <span data-ttu-id="3bc7b-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-124">Bearer.</span></span> <span data-ttu-id="3bc7b-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="3bc7b-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bc7b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc7b-126">Request body</span></span>
<span data-ttu-id="3bc7b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bc7b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc7b-128">Response</span></span>

<span data-ttu-id="3bc7b-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos do grupo de [conectores](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3bc7b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bc7b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bc7b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc7b-131">Request</span></span>
<span data-ttu-id="3bc7b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```

##### <a name="response"></a><span data-ttu-id="3bc7b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc7b-133">Response</span></span>
<span data-ttu-id="3bc7b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-134">The following is an example of the response.</span></span> <span data-ttu-id="3bc7b-135">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3bc7b-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bc7b-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": false,
      "region": "region-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
