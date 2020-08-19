---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 4ffa039d326c243dbabc9673a15711cea775e26a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807308"
---
# <a name="get-icon"></a><span data-ttu-id="0a4de-103">Get Icon</span><span class="sxs-lookup"><span data-stu-id="0a4de-103">Get Icon</span></span>

<span data-ttu-id="0a4de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a4de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a4de-105">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="0a4de-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a4de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a4de-106">Permissions</span></span>
<span data-ttu-id="0a4de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a4de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a4de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a4de-109">Permission type</span></span>      | <span data-ttu-id="0a4de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a4de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a4de-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a4de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a4de-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a4de-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a4de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a4de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a4de-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a4de-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a4de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a4de-115">Application</span></span> | <span data-ttu-id="0a4de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a4de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a4de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a4de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a4de-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a4de-118">Optional query parameters</span></span>
<span data-ttu-id="0a4de-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a4de-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a4de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a4de-120">Request headers</span></span>
| <span data-ttu-id="0a4de-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0a4de-121">Name</span></span>      |<span data-ttu-id="0a4de-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a4de-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a4de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a4de-123">Authorization</span></span>  | <span data-ttu-id="0a4de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a4de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a4de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a4de-126">Request body</span></span>
<span data-ttu-id="0a4de-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a4de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a4de-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a4de-128">Response</span></span>

<span data-ttu-id="0a4de-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookIcon](../resources/workbookicon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a4de-129">If successful, this method returns a `200 OK` response code and [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a4de-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a4de-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a4de-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a4de-131">Request</span></span>
<span data-ttu-id="0a4de-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a4de-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="0a4de-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a4de-133">Response</span></span>
<span data-ttu-id="0a4de-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a4de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
