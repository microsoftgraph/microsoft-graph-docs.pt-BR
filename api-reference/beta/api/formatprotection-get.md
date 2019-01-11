---
title: Obter FormatProtection
description: Recupere as propriedades e os relacionamentos do objeto formatprotection.
localization_priority: Normal
ms.openlocfilehash: c8588e6fc33c1fe5b1bf761a6408b1e3d2f77b8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883696"
---
# <a name="get-formatprotection"></a><span data-ttu-id="8d25c-103">Obter FormatProtection</span><span class="sxs-lookup"><span data-stu-id="8d25c-103">Get FormatProtection</span></span>

> <span data-ttu-id="8d25c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d25c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d25c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d25c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d25c-106">Recupere as propriedades e os relacionamentos do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="8d25c-106">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d25c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d25c-107">Permissions</span></span>
<span data-ttu-id="8d25c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d25c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d25c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d25c-110">Permission type</span></span>      | <span data-ttu-id="8d25c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d25c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d25c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d25c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d25c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d25c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d25c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d25c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d25c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d25c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d25c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d25c-116">Application</span></span> | <span data-ttu-id="8d25c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d25c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d25c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d25c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d25c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d25c-119">Optional query parameters</span></span>
<span data-ttu-id="8d25c-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d25c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d25c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d25c-121">Request headers</span></span>
| <span data-ttu-id="8d25c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8d25c-122">Name</span></span>      |<span data-ttu-id="8d25c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d25c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d25c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d25c-124">Authorization</span></span>  | <span data-ttu-id="8d25c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d25c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d25c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d25c-127">Request body</span></span>
<span data-ttu-id="8d25c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d25c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d25c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d25c-129">Response</span></span>

<span data-ttu-id="8d25c-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d25c-130">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d25c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d25c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d25c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d25c-132">Request</span></span>
<span data-ttu-id="8d25c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d25c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="8d25c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d25c-134">Response</span></span>
<span data-ttu-id="8d25c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d25c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
