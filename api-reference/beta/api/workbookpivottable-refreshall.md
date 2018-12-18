---
title: 'workbookPivotTable: refreshAll'
description: Atualiza a tabela dinâmica dentro de uma determinada planilha.
author: lumine2008
ms.openlocfilehash: 08a4015d58e68a3099448be91537b7970d5c1ddd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308222"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="4b747-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="4b747-103">workbookPivotTable: refreshAll</span></span>

> <span data-ttu-id="4b747-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b747-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b747-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b747-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b747-106">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="4b747-106">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b747-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b747-107">Permissions</span></span>
<span data-ttu-id="4b747-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b747-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b747-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b747-110">Permission type</span></span>      | <span data-ttu-id="4b747-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b747-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b747-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b747-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b747-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b747-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b747-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b747-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b747-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b747-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b747-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b747-116">Application</span></span> | <span data-ttu-id="4b747-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b747-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b747-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b747-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="4b747-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b747-119">Request headers</span></span>
| <span data-ttu-id="4b747-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4b747-120">Name</span></span>       | <span data-ttu-id="4b747-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b747-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b747-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b747-122">Authorization</span></span>  | <span data-ttu-id="4b747-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b747-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b747-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4b747-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4b747-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4b747-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b747-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b747-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4b747-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b747-129">Response</span></span>

<span data-ttu-id="4b747-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b747-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b747-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b747-132">Example</span></span>
<span data-ttu-id="4b747-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4b747-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b747-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b747-134">Request</span></span>
<span data-ttu-id="4b747-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b747-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="4b747-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b747-136">Response</span></span>
<span data-ttu-id="4b747-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b747-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
