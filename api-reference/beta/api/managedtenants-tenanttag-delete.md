---
title: Excluir tenantTag
description: Exclui um objeto tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e37bb368f5cd31222c1b3eaabd26fac3a5105fc7
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401977"
---
# <a name="delete-tenanttag"></a><span data-ttu-id="cecee-103">Excluir tenantTag</span><span class="sxs-lookup"><span data-stu-id="cecee-103">Delete tenantTag</span></span>
<span data-ttu-id="cecee-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="cecee-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cecee-105">Exclui um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="cecee-105">Deletes a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cecee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cecee-106">Permissions</span></span>
<span data-ttu-id="cecee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cecee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cecee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cecee-109">Permission type</span></span>|<span data-ttu-id="cecee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cecee-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cecee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cecee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cecee-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="cecee-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="cecee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cecee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cecee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cecee-114">Not supported.</span></span>|
|<span data-ttu-id="cecee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cecee-115">Application</span></span>|<span data-ttu-id="cecee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cecee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cecee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cecee-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="cecee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cecee-118">Request headers</span></span>
|<span data-ttu-id="cecee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cecee-119">Name</span></span>|<span data-ttu-id="cecee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cecee-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cecee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cecee-121">Authorization</span></span>|<span data-ttu-id="cecee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cecee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cecee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cecee-124">Request body</span></span>
<span data-ttu-id="cecee-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cecee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cecee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cecee-126">Response</span></span>

<span data-ttu-id="cecee-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cecee-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cecee-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cecee-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cecee-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cecee-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tenanttag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```


### <a name="response"></a><span data-ttu-id="cecee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cecee-130">Response</span></span>
><span data-ttu-id="cecee-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cecee-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
