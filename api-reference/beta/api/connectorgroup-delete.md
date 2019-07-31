---
title: Excluir um ou de conector
description: Excluir um conector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e8c7d0dc61338b10451f553421b74ad1b41f628f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943474"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="b7e0f-103">Excluir um ou de conector</span><span class="sxs-lookup"><span data-stu-id="b7e0f-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7e0f-104">Excluir um conector.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7e0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7e0f-105">Permissions</span></span>
<span data-ttu-id="b7e0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7e0f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7e0f-108">Permission type</span></span>      | <span data-ttu-id="b7e0f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7e0f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7e0f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7e0f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7e0f-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7e0f-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7e0f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7e0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-113">Not supported.</span></span>    |
|<span data-ttu-id="b7e0f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7e0f-114">Application</span></span> | <span data-ttu-id="b7e0f-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e0f-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="b7e0f-116">**Observação:** O grupo de conectores não deve ter conectores associados a ele.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="b7e0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7e0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7e0f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7e0f-118">Request headers</span></span>
| <span data-ttu-id="b7e0f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b7e0f-119">Name</span></span>       | <span data-ttu-id="b7e0f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7e0f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7e0f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7e0f-121">Authorization</span></span>  | <span data-ttu-id="b7e0f-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-122">Bearer.</span></span> <span data-ttu-id="b7e0f-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b7e0f-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7e0f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7e0f-124">Request body</span></span>
<span data-ttu-id="b7e0f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7e0f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7e0f-126">Response</span></span>

<span data-ttu-id="b7e0f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7e0f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7e0f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7e0f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7e0f-130">Request</span></span>
<span data-ttu-id="b7e0f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="b7e0f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7e0f-132">Response</span></span>
<span data-ttu-id="b7e0f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7e0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
