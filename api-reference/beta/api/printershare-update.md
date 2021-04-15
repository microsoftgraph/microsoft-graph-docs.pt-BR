---
title: Atualizar o printershare
description: Atualize as propriedades do compartilhamento de impressora. Esse método pode ser usado para "trocar" impressoras.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 81f5f9e6742ad19ea6d9966f92729876a1eb95eb
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766403"
---
# <a name="update-printershare"></a><span data-ttu-id="91ec8-104">Atualizar o printershare</span><span class="sxs-lookup"><span data-stu-id="91ec8-104">Update printershare</span></span>

<span data-ttu-id="91ec8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91ec8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91ec8-106">Atualize as propriedades de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="91ec8-106">Update the properties of a printer share.</span></span> <span data-ttu-id="91ec8-107">Esse método pode ser usado para trocar [impressoras](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="91ec8-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="91ec8-108">Por exemplo, se um dispositivo de impressora física [](../resources/printer.md) quebra, um administrador pode registrar um novo dispositivo de impressora e atualizar essa [impressoraShare](../resources/printerShare.md) para apontar para a nova impressora sem exigir que os usuários tomem qualquer ação.</span><span class="sxs-lookup"><span data-stu-id="91ec8-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="91ec8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="91ec8-109">Permissions</span></span>
<span data-ttu-id="91ec8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ec8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="91ec8-112">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="91ec8-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="91ec8-113">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="91ec8-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="91ec8-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91ec8-114">Permission type</span></span> | <span data-ttu-id="91ec8-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91ec8-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="91ec8-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91ec8-116">Delegated (work or school account)</span></span>| <span data-ttu-id="91ec8-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ec8-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="91ec8-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91ec8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91ec8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91ec8-119">Not Supported.</span></span>|
|<span data-ttu-id="91ec8-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91ec8-120">Application</span></span>|<span data-ttu-id="91ec8-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91ec8-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91ec8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91ec8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/shares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91ec8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91ec8-123">Request headers</span></span>
| <span data-ttu-id="91ec8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="91ec8-124">Name</span></span>       | <span data-ttu-id="91ec8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ec8-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="91ec8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="91ec8-126">Authorization</span></span> | <span data-ttu-id="91ec8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91ec8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91ec8-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="91ec8-129">Content-type</span></span>  | <span data-ttu-id="91ec8-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91ec8-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91ec8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91ec8-132">Request body</span></span>
<span data-ttu-id="91ec8-133">No corpo da solicitação, fornece os valores para campos [printerShare](../resources/printershare.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="91ec8-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="91ec8-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="91ec8-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="91ec8-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="91ec8-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="91ec8-136">As seguintes propriedades podem ser atualizadas:</span><span class="sxs-lookup"><span data-stu-id="91ec8-136">Following properties can be updated:</span></span> 

| <span data-ttu-id="91ec8-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91ec8-137">Property</span></span>     | <span data-ttu-id="91ec8-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="91ec8-138">Type</span></span>        | <span data-ttu-id="91ec8-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ec8-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91ec8-140">printer</span><span class="sxs-lookup"><span data-stu-id="91ec8-140">printer</span></span>|<span data-ttu-id="91ec8-141">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="91ec8-141">microsoft.graph.printer</span></span>|<span data-ttu-id="91ec8-142">A impressora à que essa impressora está relacionada.</span><span class="sxs-lookup"><span data-stu-id="91ec8-142">The printer that this printer share is related to.</span></span> <span data-ttu-id="91ec8-143">Use a sintaxe conforme mostrado no exemplo a seguir para atualizar a impressora à qual esse compartilhamento de impressora `printer@odata.bind` está associado.</span><span class="sxs-lookup"><span data-stu-id="91ec8-143">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|
|<span data-ttu-id="91ec8-144">displayName</span><span class="sxs-lookup"><span data-stu-id="91ec8-144">displayName</span></span>|<span data-ttu-id="91ec8-145">String</span><span class="sxs-lookup"><span data-stu-id="91ec8-145">String</span></span>|<span data-ttu-id="91ec8-146">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="91ec8-146">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="91ec8-147">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="91ec8-147">allowAllUsers</span></span>|<span data-ttu-id="91ec8-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="91ec8-148">Boolean</span></span>| <span data-ttu-id="91ec8-149">Se for true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="91ec8-149">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="91ec8-150">Isso sobressalta as listas de permissão definidas pelas propriedades de navegação allowedUsers e allowedGroups.</span><span class="sxs-lookup"><span data-stu-id="91ec8-150">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|

## <a name="response"></a><span data-ttu-id="91ec8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ec8-151">Response</span></span>
<span data-ttu-id="91ec8-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [printerShare](../resources/printershare.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91ec8-152">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91ec8-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91ec8-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91ec8-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91ec8-154">Request</span></span>
<span data-ttu-id="91ec8-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91ec8-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91ec8-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="91ec8-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/shares/{id}
Content-type: application/json
Content-length: 109

{
  "displayName": "ShareName",
  "allowAllUsers": true,
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="91ec8-157">C#</span><span class="sxs-lookup"><span data-stu-id="91ec8-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91ec8-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91ec8-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91ec8-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91ec8-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91ec8-160">Java</span><span class="sxs-lookup"><span data-stu-id="91ec8-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91ec8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ec8-161">Response</span></span>
<span data-ttu-id="91ec8-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91ec8-162">The following is an example of the response.</span></span>
><span data-ttu-id="91ec8-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91ec8-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": true,
  "status": {
    "state": "stopped",
    "details": ["disconnected"],
    "description": ""
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printershare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
