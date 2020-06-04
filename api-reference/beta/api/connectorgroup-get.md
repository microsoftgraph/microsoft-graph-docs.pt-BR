---
title: Obter um conector de conexão
description: Recupere as propriedades de um objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d487874241d6a557cd9548a7501f0a27b9b11f9
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556055"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="0be51-103">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="0be51-103">Get connectorGroup</span></span>

<span data-ttu-id="0be51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0be51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0be51-105">Recupere as propriedades de um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="0be51-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0be51-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0be51-106">Permissions</span></span>
<span data-ttu-id="0be51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be51-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0be51-109">Permission type</span></span>      | <span data-ttu-id="0be51-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0be51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0be51-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0be51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0be51-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0be51-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0be51-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0be51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0be51-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be51-114">Not supported.</span></span>    |
|<span data-ttu-id="0be51-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0be51-115">Application</span></span> | <span data-ttu-id="0be51-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be51-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0be51-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0be51-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0be51-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0be51-118">Optional query parameters</span></span>
<span data-ttu-id="0be51-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0be51-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0be51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0be51-120">Request headers</span></span>
| <span data-ttu-id="0be51-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0be51-121">Name</span></span>      |<span data-ttu-id="0be51-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0be51-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0be51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0be51-123">Authorization</span></span>  | <span data-ttu-id="0be51-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="0be51-124">Bearer.</span></span> <span data-ttu-id="0be51-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="0be51-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0be51-126">Request body</span></span>
<span data-ttu-id="0be51-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0be51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0be51-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be51-128">Response</span></span>

<span data-ttu-id="0be51-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de [teleconnector](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0be51-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be51-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0be51-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0be51-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0be51-131">Request</span></span>
<span data-ttu-id="0be51-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0be51-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="0be51-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be51-133">Response</span></span>
<span data-ttu-id="0be51-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0be51-134">The following is an example of the response.</span></span> <span data-ttu-id="0be51-135">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0be51-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0be51-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0be51-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
