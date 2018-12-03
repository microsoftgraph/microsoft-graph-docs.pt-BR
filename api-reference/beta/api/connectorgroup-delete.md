---
title: Excluir connectorGroup
description: Exclua um connectorGroup.
ms.openlocfilehash: 3ba4a5a06e25f2fb1568ab9d7d6e92104ea083de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034047"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="d5b6f-103">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d5b6f-103">Delete connectorGroup</span></span>

> <span data-ttu-id="d5b6f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5b6f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5b6f-106">Exclua um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-106">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5b6f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5b6f-107">Permissions</span></span>
<span data-ttu-id="d5b6f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5b6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5b6f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5b6f-110">Permission type</span></span>      | <span data-ttu-id="d5b6f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5b6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5b6f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5b6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5b6f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5b6f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5b6f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5b6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5b6f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-115">Not supported.</span></span>    |
|<span data-ttu-id="d5b6f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5b6f-116">Application</span></span> | <span data-ttu-id="d5b6f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b6f-117">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d5b6f-118">**Observação:** O grupo de conector não deve ter todos os conectores associados a ele.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-118">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5b6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b6f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d5b6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b6f-120">Request headers</span></span>
| <span data-ttu-id="d5b6f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d5b6f-121">Name</span></span>       | <span data-ttu-id="d5b6f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b6f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5b6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5b6f-123">Authorization</span></span>  | <span data-ttu-id="d5b6f-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-124">Bearer.</span></span> <span data-ttu-id="d5b6f-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="d5b6f-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5b6f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b6f-126">Request body</span></span>
<span data-ttu-id="d5b6f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5b6f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b6f-128">Response</span></span>

<span data-ttu-id="d5b6f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5b6f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5b6f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5b6f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b6f-132">Request</span></span>
<span data-ttu-id="d5b6f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="d5b6f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b6f-134">Response</span></span>
<span data-ttu-id="d5b6f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5b6f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
