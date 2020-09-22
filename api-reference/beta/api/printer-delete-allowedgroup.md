---
title: Excluir o permitido da impressora
description: Revoga o acesso do grupo especificado para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 581239a1bb1571d2d4636fb88af17105717ecb07
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035747"
---
# <a name="delete-allowedgroup-from-printer"></a><span data-ttu-id="e5235-103">Excluir o permitido da impressora</span><span class="sxs-lookup"><span data-stu-id="e5235-103">Delete allowedGroup from printer</span></span>

<span data-ttu-id="e5235-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5235-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5235-105">Revoga o acesso do grupo especificado para enviar trabalhos de impressão à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="e5235-105">Revoke the specified group's access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5235-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5235-106">Permissions</span></span>
<span data-ttu-id="e5235-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e5235-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e5235-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e5235-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="e5235-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e5235-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5235-111">Permission type</span></span> | <span data-ttu-id="e5235-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5235-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e5235-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5235-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e5235-114">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="e5235-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="e5235-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5235-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5235-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5235-116">Not Supported.</span></span>|
|<span data-ttu-id="e5235-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5235-117">Application</span></span>| <span data-ttu-id="e5235-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5235-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5235-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5235-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e5235-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5235-120">Request headers</span></span>
| <span data-ttu-id="e5235-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e5235-121">Name</span></span>          | <span data-ttu-id="e5235-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5235-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e5235-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5235-123">Authorization</span></span> | <span data-ttu-id="e5235-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5235-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5235-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5235-126">Request body</span></span>
<span data-ttu-id="e5235-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5235-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5235-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5235-128">Response</span></span>
<span data-ttu-id="e5235-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5235-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5235-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5235-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5235-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5235-132">Request</span></span>
<span data-ttu-id="e5235-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5235-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}/allowedGroup/{id}/$ref
```
##### <a name="response"></a><span data-ttu-id="e5235-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5235-134">Response</span></span>
<span data-ttu-id="e5235-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5235-135">The following is an example of the response.</span></span>
><span data-ttu-id="e5235-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5235-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


