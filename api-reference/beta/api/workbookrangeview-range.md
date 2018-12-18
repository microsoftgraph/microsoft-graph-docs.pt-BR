---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
ms.openlocfilehash: 22758e61f22a4275a80bf66089beaac427b2c12c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333821"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="12174-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="12174-103">workbookRangeView: range</span></span>

> <span data-ttu-id="12174-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="12174-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12174-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12174-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12174-106">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="12174-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="12174-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="12174-107">Permissions</span></span>
<span data-ttu-id="12174-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12174-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12174-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12174-110">Permission type</span></span>      | <span data-ttu-id="12174-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12174-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12174-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12174-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12174-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12174-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12174-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12174-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12174-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12174-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12174-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12174-116">Application</span></span> | <span data-ttu-id="12174-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12174-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12174-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12174-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="12174-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12174-119">Request headers</span></span>
| <span data-ttu-id="12174-120">Nome</span><span class="sxs-lookup"><span data-stu-id="12174-120">Name</span></span>       | <span data-ttu-id="12174-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="12174-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12174-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12174-122">Authorization</span></span>  | <span data-ttu-id="12174-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12174-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12174-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="12174-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="12174-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="12174-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12174-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12174-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="12174-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="12174-129">Response</span></span>

<span data-ttu-id="12174-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12174-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12174-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12174-131">Example</span></span>
<span data-ttu-id="12174-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="12174-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12174-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12174-133">Request</span></span>
<span data-ttu-id="12174-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12174-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="12174-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="12174-135">Response</span></span>
<span data-ttu-id="12174-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12174-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
