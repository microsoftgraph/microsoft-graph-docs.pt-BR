---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 616d65c490f7691ec8ab83ffd12eaba480f4734a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970901"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="e368f-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="e368f-103">workbookRangeView: range</span></span>

> <span data-ttu-id="e368f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e368f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e368f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e368f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e368f-106">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="e368f-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e368f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e368f-107">Permissions</span></span>
<span data-ttu-id="e368f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e368f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e368f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e368f-110">Permission type</span></span>      | <span data-ttu-id="e368f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e368f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e368f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e368f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e368f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e368f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e368f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e368f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e368f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e368f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e368f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e368f-116">Application</span></span> | <span data-ttu-id="e368f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e368f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e368f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e368f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="e368f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e368f-119">Request headers</span></span>
| <span data-ttu-id="e368f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e368f-120">Name</span></span>       | <span data-ttu-id="e368f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e368f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e368f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e368f-122">Authorization</span></span>  | <span data-ttu-id="e368f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e368f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e368f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e368f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e368f-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e368f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e368f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e368f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e368f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e368f-129">Response</span></span>

<span data-ttu-id="e368f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e368f-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e368f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e368f-131">Example</span></span>
<span data-ttu-id="e368f-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e368f-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e368f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e368f-133">Request</span></span>
<span data-ttu-id="e368f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e368f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="e368f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e368f-135">Response</span></span>
<span data-ttu-id="e368f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e368f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
