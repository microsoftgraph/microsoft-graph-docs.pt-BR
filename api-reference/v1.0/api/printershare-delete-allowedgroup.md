---
title: Excluir allowedGroup de printerShare
description: Revogar o acesso do grupo especificado para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 18e4ff248368cf79836797566ae6a8846d2c70d9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516900"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="1936b-103">Excluir allowedGroup de printerShare</span><span class="sxs-lookup"><span data-stu-id="1936b-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="1936b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1936b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1936b-105">Revogar o acesso do grupo especificado para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="1936b-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1936b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1936b-106">Permissions</span></span>
<span data-ttu-id="1936b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1936b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1936b-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1936b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="1936b-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="1936b-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1936b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1936b-111">Permission type</span></span> | <span data-ttu-id="1936b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1936b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1936b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1936b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1936b-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1936b-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="1936b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1936b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1936b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1936b-116">Not Supported.</span></span>|
|<span data-ttu-id="1936b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1936b-117">Application</span></span>|<span data-ttu-id="1936b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1936b-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1936b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1936b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{printerShareId}/allowedGroups/{groupId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1936b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1936b-120">Request headers</span></span>
| <span data-ttu-id="1936b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1936b-121">Name</span></span>          | <span data-ttu-id="1936b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1936b-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1936b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1936b-123">Authorization</span></span> | <span data-ttu-id="1936b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1936b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1936b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1936b-126">Request body</span></span>
<span data-ttu-id="1936b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1936b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1936b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1936b-128">Response</span></span>
<span data-ttu-id="1936b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1936b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1936b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1936b-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="1936b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1936b-132">Request</span></span>
<span data-ttu-id="1936b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1936b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/{groupId}/$ref
```
### <a name="response"></a><span data-ttu-id="1936b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1936b-134">Response</span></span>
<span data-ttu-id="1936b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1936b-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

