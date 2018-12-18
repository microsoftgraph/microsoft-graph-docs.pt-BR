---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
ms.openlocfilehash: 393f1710b82cdeed76cb0df5782d656ebb0ca9f6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355857"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="1d7ff-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="1d7ff-103">workbookPivotTable: refresh</span></span>

> <span data-ttu-id="1d7ff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d7ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d7ff-106">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-106">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="1d7ff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d7ff-107">Permissions</span></span>
<span data-ttu-id="1d7ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d7ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d7ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d7ff-110">Permission type</span></span>      | <span data-ttu-id="1d7ff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d7ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d7ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d7ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d7ff-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7ff-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d7ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d7ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d7ff-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7ff-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d7ff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d7ff-116">Application</span></span> | <span data-ttu-id="1d7ff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d7ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d7ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="1d7ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7ff-119">Request headers</span></span>
| <span data-ttu-id="1d7ff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1d7ff-120">Name</span></span>       | <span data-ttu-id="1d7ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d7ff-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d7ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d7ff-122">Authorization</span></span>  | <span data-ttu-id="1d7ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d7ff-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1d7ff-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1d7ff-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d7ff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7ff-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1d7ff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d7ff-129">Response</span></span>

<span data-ttu-id="1d7ff-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d7ff-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d7ff-132">Example</span></span>
<span data-ttu-id="1d7ff-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d7ff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7ff-134">Request</span></span>
<span data-ttu-id="1d7ff-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="1d7ff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d7ff-136">Response</span></span>
<span data-ttu-id="1d7ff-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
