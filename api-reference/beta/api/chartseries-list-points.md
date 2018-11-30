---
title: Listar pontos
description: Recupera uma lista de objetos chartpoints.
ms.openlocfilehash: 224a99ff9823522cf903339133f5ab91d76175db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035937"
---
# <a name="list-points"></a><span data-ttu-id="70c68-103">Listar pontos</span><span class="sxs-lookup"><span data-stu-id="70c68-103">List points</span></span>

> <span data-ttu-id="70c68-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="70c68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70c68-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70c68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70c68-106">Recupera uma lista de objetos chartpoints.</span><span class="sxs-lookup"><span data-stu-id="70c68-106">Retrieve a list of chartpoints objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="70c68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="70c68-107">Permissions</span></span>
<span data-ttu-id="70c68-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70c68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70c68-110">Permission type</span></span>      | <span data-ttu-id="70c68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70c68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70c68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70c68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70c68-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70c68-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70c68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70c68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70c68-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70c68-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70c68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70c68-116">Application</span></span> | <span data-ttu-id="70c68-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70c68-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70c68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70c68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70c68-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70c68-119">Optional query parameters</span></span>
<span data-ttu-id="70c68-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70c68-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70c68-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70c68-121">Request headers</span></span>
| <span data-ttu-id="70c68-122">Nome</span><span class="sxs-lookup"><span data-stu-id="70c68-122">Name</span></span>      |<span data-ttu-id="70c68-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="70c68-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70c68-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="70c68-124">Authorization</span></span>  | <span data-ttu-id="70c68-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70c68-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70c68-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="70c68-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="70c68-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="70c68-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c68-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70c68-130">Request body</span></span>
<span data-ttu-id="70c68-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70c68-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70c68-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="70c68-132">Response</span></span>

<span data-ttu-id="70c68-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ChartPoints](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70c68-133">If successful, this method returns a `200 OK` response code and collection of [ChartPoints](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70c68-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70c68-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70c68-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70c68-135">Request</span></span>
<span data-ttu-id="70c68-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70c68-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_points"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
##### <a name="response"></a><span data-ttu-id="70c68-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="70c68-137">Response</span></span>
<span data-ttu-id="70c68-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70c68-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 32

{
  "value": [
    {
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List points",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->