---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f8ff306359675f7bc2c569f507dbcb3baf33b384
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832225"
---
# <a name="get-directoryrole"></a><span data-ttu-id="34885-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="34885-103">Get directoryRole</span></span>

<span data-ttu-id="34885-104">Recupere as propriedades de um objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="34885-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34885-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34885-105">Permissions</span></span>
<span data-ttu-id="34885-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34885-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34885-108">Permission type</span></span>      | <span data-ttu-id="34885-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34885-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34885-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34885-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34885-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="34885-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="34885-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34885-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34885-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34885-113">Not supported.</span></span>    |
|<span data-ttu-id="34885-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34885-114">Application</span></span> | <span data-ttu-id="34885-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34885-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34885-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34885-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34885-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34885-117">Optional query parameters</span></span>
<span data-ttu-id="34885-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="34885-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34885-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34885-119">Request headers</span></span>
| <span data-ttu-id="34885-120">Nome</span><span class="sxs-lookup"><span data-stu-id="34885-120">Name</span></span>       | <span data-ttu-id="34885-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="34885-121">Type</span></span> | <span data-ttu-id="34885-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="34885-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34885-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34885-123">Authorization</span></span>  | <span data-ttu-id="34885-124">string</span><span class="sxs-lookup"><span data-stu-id="34885-124">string</span></span>  | <span data-ttu-id="34885-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34885-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34885-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34885-127">Request body</span></span>
<span data-ttu-id="34885-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34885-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34885-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34885-129">Response</span></span>

<span data-ttu-id="34885-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34885-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34885-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34885-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34885-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34885-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="34885-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="34885-133">Response</span></span>
<span data-ttu-id="34885-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34885-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
