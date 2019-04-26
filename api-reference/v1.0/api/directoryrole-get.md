---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ddad0f7bd6c62544dcc2aa65ede6c6db93dbd5e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550690"
---
# <a name="get-directoryrole"></a><span data-ttu-id="510a4-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="510a4-103">Get directoryRole</span></span>

<span data-ttu-id="510a4-104">Recupere as propriedades de um objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="510a4-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="510a4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="510a4-105">Permissions</span></span>
<span data-ttu-id="510a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="510a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="510a4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="510a4-108">Permission type</span></span>      | <span data-ttu-id="510a4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="510a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="510a4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="510a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="510a4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="510a4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="510a4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="510a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="510a4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="510a4-113">Not supported.</span></span>    |
|<span data-ttu-id="510a4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="510a4-114">Application</span></span> | <span data-ttu-id="510a4-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="510a4-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="510a4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="510a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="510a4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="510a4-117">Optional query parameters</span></span>
<span data-ttu-id="510a4-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="510a4-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="510a4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="510a4-119">Request headers</span></span>
| <span data-ttu-id="510a4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="510a4-120">Name</span></span>       | <span data-ttu-id="510a4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="510a4-121">Type</span></span> | <span data-ttu-id="510a4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="510a4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="510a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="510a4-123">Authorization</span></span>  | <span data-ttu-id="510a4-124">string</span><span class="sxs-lookup"><span data-stu-id="510a4-124">string</span></span>  | <span data-ttu-id="510a4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="510a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="510a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="510a4-127">Request body</span></span>
<span data-ttu-id="510a4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="510a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="510a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="510a4-129">Response</span></span>

<span data-ttu-id="510a4-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="510a4-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="510a4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="510a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="510a4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="510a4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="510a4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="510a4-133">Response</span></span>
<span data-ttu-id="510a4-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="510a4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
