---
title: Excluir o permitido de printerShare
description: Revoga o acesso do grupo especificado para enviar trabalhos de impressão ao compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8af0fd030bf438f8126e593cefe2df4cc9c5c38e
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313455"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="8ce92-103">Excluir o permitido de printerShare</span><span class="sxs-lookup"><span data-stu-id="8ce92-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="8ce92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ce92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce92-105">Revoga o acesso do grupo especificado para enviar trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="8ce92-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ce92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ce92-106">Permissions</span></span>
<span data-ttu-id="8ce92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ce92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8ce92-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8ce92-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="8ce92-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="8ce92-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8ce92-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ce92-111">Permission type</span></span> | <span data-ttu-id="8ce92-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ce92-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8ce92-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ce92-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8ce92-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ce92-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="8ce92-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ce92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ce92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ce92-116">Not Supported.</span></span>|
|<span data-ttu-id="8ce92-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ce92-117">Application</span></span>|<span data-ttu-id="8ce92-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ce92-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ce92-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ce92-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8ce92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ce92-120">Request headers</span></span>
| <span data-ttu-id="8ce92-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8ce92-121">Name</span></span>          | <span data-ttu-id="8ce92-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ce92-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8ce92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ce92-123">Authorization</span></span> | <span data-ttu-id="8ce92-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ce92-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ce92-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ce92-126">Request body</span></span>
<span data-ttu-id="8ce92-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ce92-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ce92-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ce92-128">Response</span></span>
<span data-ttu-id="8ce92-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ce92-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ce92-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ce92-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ce92-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ce92-132">Request</span></span>
<span data-ttu-id="8ce92-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ce92-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroup/{id}/$ref
```
##### <a name="response"></a><span data-ttu-id="8ce92-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ce92-134">Response</span></span>
<span data-ttu-id="8ce92-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ce92-135">The following is an example of the response.</span></span>
><span data-ttu-id="8ce92-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ce92-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->