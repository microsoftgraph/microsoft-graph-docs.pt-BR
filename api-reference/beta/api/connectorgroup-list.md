---
title: Listar connectorGroups
description: Recupere uma lista de objetos de conexão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9b18fec85e36e662ae92e5e5f70f3c14a67709a3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437375"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="6fc0a-103">Listar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="6fc0a-103">List connectorGroups</span></span>

<span data-ttu-id="6fc0a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6fc0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc0a-105">Recupere uma lista de objetos de conexão.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-105">Retrieve a list of connectorgroup objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fc0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fc0a-106">Permissions</span></span>
<span data-ttu-id="6fc0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fc0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fc0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fc0a-109">Permission type</span></span>      | <span data-ttu-id="6fc0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fc0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fc0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fc0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6fc0a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6fc0a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6fc0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fc0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fc0a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-114">Not supported.</span></span>    |
|<span data-ttu-id="6fc0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fc0a-115">Application</span></span> | <span data-ttu-id="6fc0a-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fc0a-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fc0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fc0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fc0a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6fc0a-118">Optional query parameters</span></span>
<span data-ttu-id="6fc0a-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fc0a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fc0a-120">Request headers</span></span>
| <span data-ttu-id="6fc0a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6fc0a-121">Name</span></span>      |<span data-ttu-id="6fc0a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fc0a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6fc0a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fc0a-123">Authorization</span></span>  | <span data-ttu-id="6fc0a-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-124">Bearer.</span></span> <span data-ttu-id="6fc0a-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="6fc0a-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fc0a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fc0a-126">Request body</span></span>
<span data-ttu-id="6fc0a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fc0a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fc0a-128">Response</span></span>

<span data-ttu-id="6fc0a-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos do grupo de [conectores](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fc0a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fc0a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fc0a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fc0a-131">Request</span></span>
<span data-ttu-id="6fc0a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups
```
##### <a name="response"></a><span data-ttu-id="6fc0a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fc0a-133">Response</span></span>
<span data-ttu-id="6fc0a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fc0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectorGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
