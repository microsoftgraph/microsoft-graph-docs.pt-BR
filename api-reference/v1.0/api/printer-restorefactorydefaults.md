---
title: 'printer: restoreFactoryDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 64b8db4477e79918e863b80da236e42afec83f76
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517068"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="de319-103">printer: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="de319-103">printer: restoreFactoryDefaults</span></span>
<span data-ttu-id="de319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de319-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="de319-105">Restaure [as configurações](../resources/printer.md)padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="de319-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="de319-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de319-106">Permissions</span></span>
<span data-ttu-id="de319-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="de319-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="de319-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="de319-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="de319-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="de319-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de319-111">Permission type</span></span> | <span data-ttu-id="de319-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de319-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="de319-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de319-113">Delegated (work or school account)</span></span>| <span data-ttu-id="de319-114">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="de319-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="de319-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de319-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de319-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de319-116">Not Supported.</span></span>|
|<span data-ttu-id="de319-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de319-117">Application</span></span>| <span data-ttu-id="de319-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de319-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de319-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de319-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/restoreFactoryDefaults
```

## <a name="request-headers"></a><span data-ttu-id="de319-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de319-120">Request headers</span></span>
|<span data-ttu-id="de319-121">Nome</span><span class="sxs-lookup"><span data-stu-id="de319-121">Name</span></span>|<span data-ttu-id="de319-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="de319-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de319-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de319-123">Authorization</span></span>|<span data-ttu-id="de319-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de319-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de319-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de319-126">Request body</span></span>
<span data-ttu-id="de319-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de319-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de319-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="de319-128">Response</span></span>

<span data-ttu-id="de319-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de319-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de319-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de319-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de319-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de319-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printer_restorefactorydefaults"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/restoreFactoryDefaults
```


### <a name="response"></a><span data-ttu-id="de319-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="de319-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

