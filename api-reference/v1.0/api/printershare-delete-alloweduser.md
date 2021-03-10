---
title: Excluir allowedUser de printerShare
description: Revogar o acesso do usuário especificado para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e54d4cbe1a323b80574b5865004c076e446be735
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573863"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="fd43d-103">Excluir allowedUser de printerShare</span><span class="sxs-lookup"><span data-stu-id="fd43d-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="fd43d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd43d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="fd43d-105">Revogar o acesso do usuário especificado para enviar trabalhos de impressão para a impressora [associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="fd43d-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd43d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd43d-106">Permissions</span></span>
<span data-ttu-id="fd43d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd43d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fd43d-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="fd43d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="fd43d-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="fd43d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="fd43d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd43d-111">Permission type</span></span> | <span data-ttu-id="fd43d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd43d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fd43d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd43d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="fd43d-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd43d-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="fd43d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd43d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd43d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd43d-116">Not Supported.</span></span>|
|<span data-ttu-id="fd43d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd43d-117">Application</span></span>|<span data-ttu-id="fd43d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd43d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd43d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd43d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{printerShareId}/allowedUsers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fd43d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd43d-120">Request headers</span></span>
| <span data-ttu-id="fd43d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fd43d-121">Name</span></span>          | <span data-ttu-id="fd43d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd43d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fd43d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd43d-123">Authorization</span></span> | <span data-ttu-id="fd43d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd43d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd43d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd43d-126">Request body</span></span>
<span data-ttu-id="fd43d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd43d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd43d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd43d-128">Response</span></span>
<span data-ttu-id="fd43d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd43d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd43d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd43d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd43d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd43d-132">Request</span></span>
<span data-ttu-id="fd43d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd43d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers/{userId}/$ref
```

### <a name="response"></a><span data-ttu-id="fd43d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd43d-134">Response</span></span>
<span data-ttu-id="fd43d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fd43d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
