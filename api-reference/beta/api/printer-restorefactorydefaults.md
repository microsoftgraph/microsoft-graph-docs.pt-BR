---
title: 'impressora: restoreFactoryDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9bae7ed31a9ac73fdda0f576b47129a888190811
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731103"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="011af-103">impressora: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="011af-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="011af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="011af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="011af-105">Restaurar as configurações de uma [impressora](../resources/printer.md)para as configurações de fábrica.</span><span class="sxs-lookup"><span data-stu-id="011af-105">Restore a [printer](../resources/printer.md)'s settings to the factory settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="011af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="011af-106">Permissions</span></span>
<span data-ttu-id="011af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="011af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="011af-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="011af-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="011af-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="011af-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="011af-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="011af-111">Permission type</span></span> | <span data-ttu-id="011af-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="011af-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="011af-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="011af-113">Delegated (work or school account)</span></span>| <span data-ttu-id="011af-114">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="011af-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="011af-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="011af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="011af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="011af-116">Not Supported.</span></span>|
|<span data-ttu-id="011af-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="011af-117">Application</span></span>| <span data-ttu-id="011af-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="011af-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="011af-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="011af-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="011af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="011af-120">Request headers</span></span>
| <span data-ttu-id="011af-121">Nome</span><span class="sxs-lookup"><span data-stu-id="011af-121">Name</span></span>          | <span data-ttu-id="011af-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="011af-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="011af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="011af-123">Authorization</span></span> | <span data-ttu-id="011af-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="011af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="011af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="011af-126">Request body</span></span>
<span data-ttu-id="011af-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="011af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="011af-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="011af-128">Response</span></span>
<span data-ttu-id="011af-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="011af-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="011af-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="011af-131">Example</span></span>
<span data-ttu-id="011af-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="011af-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="011af-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="011af-133">Request</span></span>
<span data-ttu-id="011af-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="011af-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```

### <a name="response"></a><span data-ttu-id="011af-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="011af-135">Response</span></span>
<span data-ttu-id="011af-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="011af-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: restoreFactoryDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
