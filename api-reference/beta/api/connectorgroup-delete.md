---
title: Excluir um ou de conector
description: Excluir um conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45b0216562ce8fefa139726446fbf3eb97daaabd
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556062"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="db2c6-103">Excluir um ou de conector</span><span class="sxs-lookup"><span data-stu-id="db2c6-103">Delete connectorGroup</span></span>

<span data-ttu-id="db2c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db2c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db2c6-105">Excluir um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="db2c6-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="db2c6-106">Todos os [conectores](../resources/connector.md) e aplicativos devem ser removidos do grupo de conectores para que um grupo de conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="db2c6-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="db2c6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="db2c6-107">Permissions</span></span>
<span data-ttu-id="db2c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db2c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db2c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db2c6-110">Permission type</span></span>      | <span data-ttu-id="db2c6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db2c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db2c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db2c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db2c6-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db2c6-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db2c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db2c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db2c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db2c6-115">Not supported.</span></span>    |
|<span data-ttu-id="db2c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db2c6-116">Application</span></span> | <span data-ttu-id="db2c6-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db2c6-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db2c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db2c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db2c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db2c6-119">Request headers</span></span>
| <span data-ttu-id="db2c6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="db2c6-120">Name</span></span>       | <span data-ttu-id="db2c6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="db2c6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db2c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db2c6-122">Authorization</span></span>  | <span data-ttu-id="db2c6-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="db2c6-123">Bearer.</span></span> <span data-ttu-id="db2c6-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="db2c6-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="db2c6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db2c6-125">Request body</span></span>
<span data-ttu-id="db2c6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db2c6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db2c6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="db2c6-127">Response</span></span>

<span data-ttu-id="db2c6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db2c6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db2c6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db2c6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db2c6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db2c6-131">Request</span></span>
<span data-ttu-id="db2c6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db2c6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="db2c6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="db2c6-133">Response</span></span>
<span data-ttu-id="db2c6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db2c6-134">The following is an example of the response.</span></span> <span data-ttu-id="db2c6-135">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="db2c6-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db2c6-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db2c6-136">All of the properties will be returned from an actual call.</span></span>
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
