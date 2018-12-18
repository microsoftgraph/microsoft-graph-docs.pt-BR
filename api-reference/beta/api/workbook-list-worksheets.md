---
title: Listar planilhas
description: Recupere uma lista de objetos de planilha.
author: lumine2008
ms.openlocfilehash: 218138a8bb9c15430c3693ab137afea9de91e059
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332988"
---
# <a name="list-worksheets"></a><span data-ttu-id="4173a-103">Listar planilhas</span><span class="sxs-lookup"><span data-stu-id="4173a-103">List worksheets</span></span>

> <span data-ttu-id="4173a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4173a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4173a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4173a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4173a-106">Recupere uma lista de objetos de planilha.</span><span class="sxs-lookup"><span data-stu-id="4173a-106">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4173a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4173a-107">Permissions</span></span>
<span data-ttu-id="4173a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4173a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4173a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4173a-110">Permission type</span></span>      | <span data-ttu-id="4173a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4173a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4173a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4173a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4173a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4173a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4173a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4173a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4173a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4173a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4173a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4173a-116">Application</span></span> | <span data-ttu-id="4173a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4173a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4173a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4173a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4173a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4173a-119">Optional query parameters</span></span>
<span data-ttu-id="4173a-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4173a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4173a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-121">Request headers</span></span>
| <span data-ttu-id="4173a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4173a-122">Name</span></span>      |<span data-ttu-id="4173a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4173a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4173a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4173a-124">Authorization</span></span>  | <span data-ttu-id="4173a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4173a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4173a-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4173a-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="4173a-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4173a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4173a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-130">Request body</span></span>
<span data-ttu-id="4173a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4173a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4173a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-132">Response</span></span>

<span data-ttu-id="4173a-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Worksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4173a-133">If successful, this method returns a `200 OK` response code and collection of [Worksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4173a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4173a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4173a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-135">Request</span></span>
<span data-ttu-id="4173a-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4173a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="4173a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-137">Response</span></span>
<span data-ttu-id="4173a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4173a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->