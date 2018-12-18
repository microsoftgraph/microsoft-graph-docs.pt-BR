---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
ms.openlocfilehash: 6e9c0c0f36231a29689c24d721d8c8978e8f1bf0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362731"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="821e4-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="821e4-103">workbookRangeView: range</span></span>
<span data-ttu-id="821e4-104">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="821e4-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="821e4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="821e4-105">Permissions</span></span>
<span data-ttu-id="821e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="821e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="821e4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="821e4-108">Permission type</span></span>      | <span data-ttu-id="821e4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="821e4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="821e4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="821e4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="821e4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="821e4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="821e4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="821e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="821e4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="821e4-113">Not supported.</span></span>    |
|<span data-ttu-id="821e4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="821e4-114">Application</span></span> | <span data-ttu-id="821e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="821e4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="821e4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="821e4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="821e4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="821e4-117">Request headers</span></span>
| <span data-ttu-id="821e4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="821e4-118">Name</span></span>       | <span data-ttu-id="821e4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="821e4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="821e4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="821e4-120">Authorization</span></span>  | <span data-ttu-id="821e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="821e4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="821e4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="821e4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="821e4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="821e4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="821e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="821e4-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="821e4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="821e4-127">Response</span></span>
<span data-ttu-id="821e4-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="821e4-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821e4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="821e4-129">Example</span></span>
<span data-ttu-id="821e4-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="821e4-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="821e4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="821e4-131">Request</span></span>
<span data-ttu-id="821e4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="821e4-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="821e4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="821e4-133">Response</span></span>
<span data-ttu-id="821e4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="821e4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
