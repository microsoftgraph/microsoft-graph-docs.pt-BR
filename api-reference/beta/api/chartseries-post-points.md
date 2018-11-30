---
title: Criar ChartPoints
description: Use essa API para criar novos ChartPoints.
ms.openlocfilehash: be10973510b053b30178a3c5b35a866f828bf927
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033356"
---
# <a name="create-chartpoints"></a><span data-ttu-id="eb6da-103">Criar ChartPoints</span><span class="sxs-lookup"><span data-stu-id="eb6da-103">Create ChartPoints</span></span>

> <span data-ttu-id="eb6da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eb6da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb6da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eb6da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb6da-106">Use essa API para criar novos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="eb6da-106">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb6da-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb6da-107">Permissions</span></span>
<span data-ttu-id="eb6da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb6da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb6da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb6da-110">Permission type</span></span>      | <span data-ttu-id="eb6da-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb6da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb6da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb6da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb6da-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb6da-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb6da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb6da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb6da-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb6da-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb6da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb6da-116">Application</span></span> | <span data-ttu-id="eb6da-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6da-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb6da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="eb6da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6da-119">Request headers</span></span>
| <span data-ttu-id="eb6da-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eb6da-120">Name</span></span>       | <span data-ttu-id="eb6da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb6da-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb6da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb6da-122">Authorization</span></span>  | <span data-ttu-id="eb6da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb6da-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb6da-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eb6da-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="eb6da-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb6da-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb6da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6da-128">Request body</span></span>
<span data-ttu-id="eb6da-129">No corpo da solicitação, forneça uma representação JSON do objeto [ChartPoints](../resources/chartpoint.md).</span><span class="sxs-lookup"><span data-stu-id="eb6da-129">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eb6da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6da-130">Response</span></span>

<span data-ttu-id="eb6da-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ChartPoints](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb6da-131">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb6da-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb6da-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb6da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6da-133">Request</span></span>
<span data-ttu-id="eb6da-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb6da-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="eb6da-135">No corpo da solicitação, forneça uma representação JSON do objeto [ChartPoints](../resources/chartpoint.md).</span><span class="sxs-lookup"><span data-stu-id="eb6da-135">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eb6da-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6da-136">Response</span></span>
<span data-ttu-id="eb6da-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb6da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->