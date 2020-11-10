---
title: Atualizar PrinterShare
description: Atualize as propriedades do compartilhamento da impressora. Este método pode ser usado para "trocar" impressoras.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: afbf37fe04eb049f399296ff6d7d74fe7d1c0f47
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968303"
---
# <a name="update-printershare"></a><span data-ttu-id="8036b-104">Atualizar PrinterShare</span><span class="sxs-lookup"><span data-stu-id="8036b-104">Update printershare</span></span>

<span data-ttu-id="8036b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8036b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8036b-106">Atualizar as propriedades de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="8036b-106">Update the properties of a printer share.</span></span> <span data-ttu-id="8036b-107">Este método pode ser usado para trocar [impressoras](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="8036b-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="8036b-108">Por exemplo, se um dispositivo de impressora física for interrompido, um administrador poderá registrar um novo dispositivo de [impressora](../resources/printer.md) e atualizar esse [printerShare](../resources/printerShare.md) para apontar para a nova impressora sem exigir que os usuários executem qualquer ação.</span><span class="sxs-lookup"><span data-stu-id="8036b-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="8036b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8036b-109">Permissions</span></span>
<span data-ttu-id="8036b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8036b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8036b-112">Além das permissões a seguir, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa.</span><span class="sxs-lookup"><span data-stu-id="8036b-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="8036b-113">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="8036b-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8036b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8036b-114">Permission type</span></span> | <span data-ttu-id="8036b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8036b-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8036b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8036b-116">Delegated (work or school account)</span></span>| <span data-ttu-id="8036b-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8036b-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="8036b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8036b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8036b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8036b-119">Not Supported.</span></span>|
|<span data-ttu-id="8036b-120">Application</span><span class="sxs-lookup"><span data-stu-id="8036b-120">Application</span></span>|<span data-ttu-id="8036b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8036b-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8036b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8036b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/shares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8036b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8036b-123">Request headers</span></span>
| <span data-ttu-id="8036b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8036b-124">Name</span></span>       | <span data-ttu-id="8036b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8036b-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8036b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8036b-126">Authorization</span></span> | <span data-ttu-id="8036b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8036b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8036b-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="8036b-129">Content-type</span></span>  | <span data-ttu-id="8036b-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8036b-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8036b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8036b-132">Request body</span></span>
<span data-ttu-id="8036b-133">No corpo da solicitação, forneça os valores para campos [printerShare](../resources/printershare.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8036b-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="8036b-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8036b-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8036b-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8036b-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8036b-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8036b-136">Property</span></span>     | <span data-ttu-id="8036b-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8036b-137">Type</span></span>        | <span data-ttu-id="8036b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8036b-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8036b-139">impressora</span><span class="sxs-lookup"><span data-stu-id="8036b-139">printer</span></span>|<span data-ttu-id="8036b-140">String</span><span class="sxs-lookup"><span data-stu-id="8036b-140">String</span></span>|<span data-ttu-id="8036b-141">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="8036b-141">The printer that this printer share is related to.</span></span> <span data-ttu-id="8036b-142">Use a `printer@odata.bind` sintaxe, conforme mostrado no exemplo a seguir, para atualizar a impressora à qual este compartilhamento de impressora está associado.</span><span class="sxs-lookup"><span data-stu-id="8036b-142">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|

><span data-ttu-id="8036b-143">**Observação:** Não há suporte para a atualização do nome de compartilhamento da impressora.</span><span class="sxs-lookup"><span data-stu-id="8036b-143">**Note:** Updating the printer share name is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="8036b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8036b-144">Response</span></span>
<span data-ttu-id="8036b-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printerShare](../resources/printershare.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8036b-145">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8036b-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8036b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8036b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8036b-147">Request</span></span>
<span data-ttu-id="8036b-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8036b-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8036b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8036b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/shares/{id}
Content-type: application/json
Content-length: 109

{
  "name": "ShareName",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="8036b-150">C#</span><span class="sxs-lookup"><span data-stu-id="8036b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8036b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8036b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8036b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8036b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8036b-153">Java</span><span class="sxs-lookup"><span data-stu-id="8036b-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8036b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="8036b-154">Response</span></span>
<span data-ttu-id="8036b-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8036b-155">The following is an example of the response.</span></span>
><span data-ttu-id="8036b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8036b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
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
