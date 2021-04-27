---
title: Criar printerShare
description: Cria um novo compartilhamento de impressora para a impressora especificada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 57d755532e2e56934f32aaa0940504073eef7473
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053626"
---
# <a name="create-printershare"></a><span data-ttu-id="cc9fd-103">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="cc9fd-103">Create printerShare</span></span>

<span data-ttu-id="cc9fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc9fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc9fd-105">Crie uma nova **printerShare** para a impressora [especificada](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="cc9fd-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc9fd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc9fd-106">Permissions</span></span>
<span data-ttu-id="cc9fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc9fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cc9fd-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="cc9fd-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="cc9fd-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="cc9fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc9fd-111">Permission type</span></span> | <span data-ttu-id="cc9fd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc9fd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cc9fd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc9fd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="cc9fd-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc9fd-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="cc9fd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc9fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc9fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-116">Not Supported.</span></span>|
|<span data-ttu-id="cc9fd-117">Application</span><span class="sxs-lookup"><span data-stu-id="cc9fd-117">Application</span></span>|<span data-ttu-id="cc9fd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc9fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc9fd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares
```
## <a name="request-headers"></a><span data-ttu-id="cc9fd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc9fd-120">Request headers</span></span>
| <span data-ttu-id="cc9fd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cc9fd-121">Name</span></span>          | <span data-ttu-id="cc9fd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc9fd-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cc9fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc9fd-123">Authorization</span></span> | <span data-ttu-id="cc9fd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc9fd-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="cc9fd-126">Content-type</span></span>  | <span data-ttu-id="cc9fd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc9fd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc9fd-129">Request body</span></span>
<span data-ttu-id="cc9fd-130">No corpo da solicitação, fornece uma representação JSON do [objeto printerShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="cc9fd-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="cc9fd-131">A tabela a seguir mostra as propriedades que podem ser fornecidas ao criar [a printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="cc9fd-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="cc9fd-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc9fd-132">Property</span></span>|<span data-ttu-id="cc9fd-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc9fd-133">Type</span></span>|<span data-ttu-id="cc9fd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc9fd-134">Description</span></span>|<span data-ttu-id="cc9fd-135">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="cc9fd-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="cc9fd-136">printer</span><span class="sxs-lookup"><span data-stu-id="cc9fd-136">printer</span></span>|<span data-ttu-id="cc9fd-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="cc9fd-137">microsoft.graph.printer</span></span>|<span data-ttu-id="cc9fd-138">A impressora à que essa impressora está relacionada.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="cc9fd-139">Use a `printer@odata.bind` sintaxe conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-139">Use the `printer@odata.bind` syntax as shown in the following example.</span></span>|<span data-ttu-id="cc9fd-140">Sim</span><span class="sxs-lookup"><span data-stu-id="cc9fd-140">Yes</span></span>|
|<span data-ttu-id="cc9fd-141">displayName</span><span class="sxs-lookup"><span data-stu-id="cc9fd-141">displayName</span></span>|<span data-ttu-id="cc9fd-142">String</span><span class="sxs-lookup"><span data-stu-id="cc9fd-142">String</span></span>|<span data-ttu-id="cc9fd-143">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="cc9fd-144">O comprimento máximo permitido é de 50 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="cc9fd-145">Sim</span><span class="sxs-lookup"><span data-stu-id="cc9fd-145">Yes</span></span>|
|<span data-ttu-id="cc9fd-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="cc9fd-146">allowAllUsers</span></span>|<span data-ttu-id="cc9fd-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc9fd-147">Boolean</span></span>| <span data-ttu-id="cc9fd-148">Se for true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-148">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="cc9fd-149">Isso sobressalta as listas de permissão definidas pelas propriedades de navegação allowedUsers e allowedGroups.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-149">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|<span data-ttu-id="cc9fd-150">Não</span><span class="sxs-lookup"><span data-stu-id="cc9fd-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="cc9fd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc9fd-151">Response</span></span>
<span data-ttu-id="cc9fd-152">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc9fd-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc9fd-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc9fd-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc9fd-154">Request</span></span>
<span data-ttu-id="cc9fd-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc9fd-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc9fd-156">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="cc9fd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc9fd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="cc9fd-158">C#</span><span class="sxs-lookup"><span data-stu-id="cc9fd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printershare-from-print-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc9fd-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc9fd-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printershare-from-print-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc9fd-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc9fd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printershare-from-print-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc9fd-161">Java</span><span class="sxs-lookup"><span data-stu-id="cc9fd-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printershare-from-print-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="cc9fd-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc9fd-162">Response</span></span>
<span data-ttu-id="cc9fd-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-163">The following is an example of the response.</span></span>
><span data-ttu-id="cc9fd-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc9fd-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "displayName": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
