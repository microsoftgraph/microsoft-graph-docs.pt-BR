---
title: Criar printerShare
description: Cria um novo compartilhamento de impressora para a impressora especificada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f22101ff6a621a48285f8064595916e491eb996d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516880"
---
# <a name="create-printershare"></a><span data-ttu-id="d09d0-103">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="d09d0-103">Create printerShare</span></span>
<span data-ttu-id="d09d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d09d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d09d0-105">Crie uma nova **printerShare** para a impressora [especificada](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="d09d0-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d09d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d09d0-106">Permissions</span></span>
<span data-ttu-id="d09d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d09d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d09d0-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d09d0-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="d09d0-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="d09d0-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="d09d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d09d0-111">Permission type</span></span> | <span data-ttu-id="d09d0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d09d0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d09d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d09d0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d09d0-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d09d0-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="d09d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d09d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d09d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d09d0-116">Not Supported.</span></span>|
|<span data-ttu-id="d09d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d09d0-117">Application</span></span>|<span data-ttu-id="d09d0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d09d0-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d09d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d09d0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares
```

## <a name="request-headers"></a><span data-ttu-id="d09d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d09d0-120">Request headers</span></span>
|<span data-ttu-id="d09d0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d09d0-121">Name</span></span>|<span data-ttu-id="d09d0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d09d0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d09d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d09d0-123">Authorization</span></span>|<span data-ttu-id="d09d0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d09d0-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d09d0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d09d0-126">Content-Type</span></span>|<span data-ttu-id="d09d0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d09d0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d09d0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d09d0-129">Request body</span></span>
<span data-ttu-id="d09d0-130">No corpo da solicitação, fornece uma representação JSON do [objeto printerShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="d09d0-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="d09d0-131">A tabela a seguir mostra as propriedades que podem ser fornecidas ao criar [a printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="d09d0-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="d09d0-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d09d0-132">Property</span></span>|<span data-ttu-id="d09d0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d09d0-133">Type</span></span>|<span data-ttu-id="d09d0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d09d0-134">Description</span></span>|<span data-ttu-id="d09d0-135">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="d09d0-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="d09d0-136">impressora</span><span class="sxs-lookup"><span data-stu-id="d09d0-136">printer</span></span>|<span data-ttu-id="d09d0-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="d09d0-137">microsoft.graph.printer</span></span>|<span data-ttu-id="d09d0-138">A impressora à que essa impressora está relacionada.</span><span class="sxs-lookup"><span data-stu-id="d09d0-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="d09d0-139">Use a `printer@odata.bind` sintaxe, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="d09d0-139">Use the `printer@odata.bind` syntax, as shown in the following example.</span></span>|<span data-ttu-id="d09d0-140">Sim</span><span class="sxs-lookup"><span data-stu-id="d09d0-140">Yes</span></span>|
|<span data-ttu-id="d09d0-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d09d0-141">displayName</span></span>|<span data-ttu-id="d09d0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d09d0-142">String</span></span>|<span data-ttu-id="d09d0-143">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="d09d0-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="d09d0-144">O comprimento máximo permitido é de 50 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d09d0-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="d09d0-145">Sim</span><span class="sxs-lookup"><span data-stu-id="d09d0-145">Yes</span></span>|
|<span data-ttu-id="d09d0-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="d09d0-146">allowAllUsers</span></span>|<span data-ttu-id="d09d0-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="d09d0-147">Boolean</span></span>|<span data-ttu-id="d09d0-148">Se `true` , todos os usuários e grupos terão acesso a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="d09d0-148">If `true`, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="d09d0-149">Isso sobressalta as listas de permissão definidas pelas propriedades de navegação **allowedUsers** e **allowedGroups.**</span><span class="sxs-lookup"><span data-stu-id="d09d0-149">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|<span data-ttu-id="d09d0-150">Não</span><span class="sxs-lookup"><span data-stu-id="d09d0-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="d09d0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d09d0-151">Response</span></span>

<span data-ttu-id="d09d0-152">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d09d0-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d09d0-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d09d0-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d09d0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d09d0-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares
Content-Type: application/json
Content-length: 509

{
  "displayName": "ShareName",
  "allowAllUsers": false,
  "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
}
```

### <a name="response"></a><span data-ttu-id="d09d0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d09d0-155">Response</span></span>
<span data-ttu-id="d09d0-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d09d0-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "status": {
    "state": "ready",
    "details": [],
    "description": ""
  }
}
```

