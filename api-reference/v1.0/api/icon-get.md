---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
ms.openlocfilehash: 4b33ba32da3130ce4ee47d58826796c4b50402fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003721"
---
# <a name="get-icon"></a><span data-ttu-id="aa6a9-103">Obter ícone</span><span class="sxs-lookup"><span data-stu-id="aa6a9-103">Get Icon</span></span>

<span data-ttu-id="aa6a9-104">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-104">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa6a9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa6a9-105">Permissions</span></span>
<span data-ttu-id="aa6a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa6a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa6a9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa6a9-108">Permission type</span></span>      | <span data-ttu-id="aa6a9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa6a9-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="aa6a9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa6a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa6a9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa6a9-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="aa6a9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa6a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa6a9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-113">Not supported.</span></span>    | 
|<span data-ttu-id="aa6a9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa6a9-114">Application</span></span> | <span data-ttu-id="aa6a9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa6a9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa6a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa6a9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa6a9-117">Optional query parameters</span></span>
<span data-ttu-id="aa6a9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa6a9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6a9-119">Request headers</span></span>
| <span data-ttu-id="aa6a9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="aa6a9-120">Name</span></span>      |<span data-ttu-id="aa6a9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa6a9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa6a9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa6a9-122">Authorization</span></span>  | <span data-ttu-id="aa6a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="aa6a9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6a9-125">Request body</span></span>
<span data-ttu-id="aa6a9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa6a9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa6a9-127">Response</span></span>

<span data-ttu-id="aa6a9-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Icon](../resources/icon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-128">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa6a9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa6a9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa6a9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6a9-130">Request</span></span>
<span data-ttu-id="aa6a9-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="aa6a9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa6a9-132">Response</span></span>
<span data-ttu-id="aa6a9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa6a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->