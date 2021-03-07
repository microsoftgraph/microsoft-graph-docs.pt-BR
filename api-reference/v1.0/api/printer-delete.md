---
title: Eliminar impressora
description: Excluir (não registro) uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2a1d1b91e5f3b68995a27021c0b2fc3eb39de939
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516908"
---
# <a name="delete-printer"></a><span data-ttu-id="2ce77-103">Eliminar impressora</span><span class="sxs-lookup"><span data-stu-id="2ce77-103">Delete printer</span></span>
<span data-ttu-id="2ce77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ce77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2ce77-105">Excluir (não registro) uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="2ce77-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce77-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ce77-106">Permissions</span></span>
<span data-ttu-id="2ce77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2ce77-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="2ce77-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2ce77-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="2ce77-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2ce77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ce77-111">Permission type</span></span> | <span data-ttu-id="2ce77-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ce77-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2ce77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ce77-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2ce77-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2ce77-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="2ce77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ce77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ce77-116">Not Supported.</span></span>|
|<span data-ttu-id="2ce77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ce77-117">Application</span></span>|<span data-ttu-id="2ce77-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ce77-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ce77-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="2ce77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ce77-120">Request headers</span></span>
|<span data-ttu-id="2ce77-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2ce77-121">Name</span></span>|<span data-ttu-id="2ce77-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ce77-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ce77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ce77-123">Authorization</span></span>|<span data-ttu-id="2ce77-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ce77-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce77-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ce77-126">Request body</span></span>
<span data-ttu-id="2ce77-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ce77-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ce77-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ce77-128">Response</span></span>

<span data-ttu-id="2ce77-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ce77-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2ce77-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ce77-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ce77-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ce77-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}
```


### <a name="response"></a><span data-ttu-id="2ce77-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ce77-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

