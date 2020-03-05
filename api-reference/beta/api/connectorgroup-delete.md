---
title: Excluir um ou de conector
description: Excluir um conector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 960fe8a61dc00eaddcd6c96e255ea7cb7033434c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437480"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="237f2-103">Excluir um ou de conector</span><span class="sxs-lookup"><span data-stu-id="237f2-103">Delete connectorGroup</span></span>

<span data-ttu-id="237f2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="237f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="237f2-105">Excluir um conector.</span><span class="sxs-lookup"><span data-stu-id="237f2-105">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="237f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="237f2-106">Permissions</span></span>
<span data-ttu-id="237f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="237f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="237f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="237f2-109">Permission type</span></span>      | <span data-ttu-id="237f2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="237f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="237f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="237f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="237f2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="237f2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="237f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="237f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="237f2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="237f2-114">Not supported.</span></span>    |
|<span data-ttu-id="237f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="237f2-115">Application</span></span> | <span data-ttu-id="237f2-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="237f2-116">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="237f2-117">**Observação:** O grupo de conectores não deve ter conectores associados a ele.</span><span class="sxs-lookup"><span data-stu-id="237f2-117">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="237f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="237f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="237f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="237f2-119">Request headers</span></span>
| <span data-ttu-id="237f2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="237f2-120">Name</span></span>       | <span data-ttu-id="237f2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="237f2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="237f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="237f2-122">Authorization</span></span>  | <span data-ttu-id="237f2-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="237f2-123">Bearer.</span></span> <span data-ttu-id="237f2-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="237f2-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="237f2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="237f2-125">Request body</span></span>
<span data-ttu-id="237f2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="237f2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="237f2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="237f2-127">Response</span></span>

<span data-ttu-id="237f2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="237f2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="237f2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="237f2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="237f2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="237f2-131">Request</span></span>
<span data-ttu-id="237f2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="237f2-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="237f2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="237f2-133">Response</span></span>
<span data-ttu-id="237f2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="237f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
