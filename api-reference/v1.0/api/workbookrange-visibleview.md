---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
ms.openlocfilehash: 1832c30c8a223b1a5067cede03796bcab16d5a94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826905"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="434fd-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="434fd-104">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="434fd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="434fd-105">Permissions</span></span>
<span data-ttu-id="434fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="434fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="434fd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="434fd-108">Permission type</span></span>      | <span data-ttu-id="434fd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="434fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="434fd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="434fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="434fd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="434fd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="434fd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="434fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="434fd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="434fd-113">Not supported.</span></span>    |
|<span data-ttu-id="434fd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="434fd-114">Application</span></span> | <span data-ttu-id="434fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="434fd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="434fd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="434fd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="434fd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="434fd-117">Request headers</span></span>
| <span data-ttu-id="434fd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="434fd-118">Name</span></span>       | <span data-ttu-id="434fd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="434fd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="434fd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="434fd-120">Authorization</span></span>  | <span data-ttu-id="434fd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="434fd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="434fd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="434fd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="434fd-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="434fd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="434fd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="434fd-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="434fd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="434fd-127">Response</span></span>
<span data-ttu-id="434fd-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="434fd-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="434fd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="434fd-129">Example</span></span>
<span data-ttu-id="434fd-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="434fd-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="434fd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="434fd-131">Request</span></span>
<span data-ttu-id="434fd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="434fd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="434fd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="434fd-133">Response</span></span>
<span data-ttu-id="434fd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="434fd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
