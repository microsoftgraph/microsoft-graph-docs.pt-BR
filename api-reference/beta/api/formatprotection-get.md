---
title: Obter FormatProtection
description: Recupere as propriedades e os relacionamentos do objeto formatprotection.
ms.openlocfilehash: 341206df02f966d6458ed1812b33443e23e71daf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035891"
---
# <a name="get-formatprotection"></a><span data-ttu-id="caaf8-103">Obter FormatProtection</span><span class="sxs-lookup"><span data-stu-id="caaf8-103">Get FormatProtection</span></span>

> <span data-ttu-id="caaf8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="caaf8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="caaf8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="caaf8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="caaf8-106">Recupere as propriedades e os relacionamentos do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="caaf8-106">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="caaf8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="caaf8-107">Permissions</span></span>
<span data-ttu-id="caaf8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caaf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caaf8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caaf8-110">Permission type</span></span>      | <span data-ttu-id="caaf8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="caaf8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caaf8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caaf8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="caaf8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caaf8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="caaf8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caaf8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caaf8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caaf8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="caaf8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caaf8-116">Application</span></span> | <span data-ttu-id="caaf8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caaf8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="caaf8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caaf8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="caaf8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="caaf8-119">Optional query parameters</span></span>
<span data-ttu-id="caaf8-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="caaf8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="caaf8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caaf8-121">Request headers</span></span>
| <span data-ttu-id="caaf8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="caaf8-122">Name</span></span>      |<span data-ttu-id="caaf8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="caaf8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="caaf8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="caaf8-124">Authorization</span></span>  | <span data-ttu-id="caaf8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caaf8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caaf8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caaf8-127">Request body</span></span>
<span data-ttu-id="caaf8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="caaf8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caaf8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="caaf8-129">Response</span></span>

<span data-ttu-id="caaf8-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caaf8-130">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="caaf8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caaf8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="caaf8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caaf8-132">Request</span></span>
<span data-ttu-id="caaf8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="caaf8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="caaf8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="caaf8-134">Response</span></span>
<span data-ttu-id="caaf8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caaf8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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