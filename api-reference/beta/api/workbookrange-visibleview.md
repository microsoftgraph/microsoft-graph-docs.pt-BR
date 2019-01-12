---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: eaa4fd44cc976281348f658eda7ecc358f19efc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952906"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="4b570-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="4b570-104">workbookRange: visibleView</span></span>

> <span data-ttu-id="4b570-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b570-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b570-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b570-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b570-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4b570-107">Permissions</span></span>
<span data-ttu-id="4b570-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b570-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b570-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b570-110">Permission type</span></span>      | <span data-ttu-id="4b570-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b570-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b570-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b570-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b570-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b570-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b570-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b570-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b570-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b570-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b570-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b570-116">Application</span></span> | <span data-ttu-id="4b570-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b570-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b570-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b570-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="4b570-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b570-119">Request headers</span></span>
| <span data-ttu-id="4b570-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4b570-120">Name</span></span>       | <span data-ttu-id="4b570-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b570-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b570-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b570-122">Authorization</span></span>  | <span data-ttu-id="4b570-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b570-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b570-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4b570-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4b570-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4b570-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b570-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b570-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4b570-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b570-129">Response</span></span>

<span data-ttu-id="4b570-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b570-130">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b570-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b570-131">Example</span></span>
<span data-ttu-id="4b570-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4b570-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b570-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b570-133">Request</span></span>
<span data-ttu-id="4b570-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b570-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="4b570-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b570-135">Response</span></span>
<span data-ttu-id="4b570-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b570-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
