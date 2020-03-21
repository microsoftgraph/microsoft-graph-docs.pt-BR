---
title: Atualizar PrinterShare
description: Atualize as propriedades do compartilhamento da impressora. Este método pode ser usado para "trocar" impressoras.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7326a37afd351fee6cce7c89663e65cb2aba5099
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895543"
---
# <a name="update-printershare"></a><span data-ttu-id="d2c9d-104">Atualizar PrinterShare</span><span class="sxs-lookup"><span data-stu-id="d2c9d-104">Update printershare</span></span>

<span data-ttu-id="d2c9d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2c9d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2c9d-106">Atualizar as propriedades de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-106">Update the properties of a printer share.</span></span> <span data-ttu-id="d2c9d-107">Este método pode ser usado para trocar [impressoras](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="d2c9d-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="d2c9d-108">Por exemplo, se um dispositivo de impressora física for interrompido, um administrador poderá registrar um novo dispositivo de [impressora](../resources/printer.md) e atualizar esse [printerShare](../resources/printerShare.md) para apontar para a nova impressora sem exigir que os usuários executem qualquer ação.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2c9d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2c9d-109">Permissions</span></span>
<span data-ttu-id="d2c9d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2c9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d2c9d-112">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-112">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d2c9d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2c9d-113">Permission type</span></span> | <span data-ttu-id="d2c9d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2c9d-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d2c9d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2c9d-115">Delegated (work or school account)</span></span>| <span data-ttu-id="d2c9d-116">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="d2c9d-116">Users.Read.All</span></span> |
|<span data-ttu-id="d2c9d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2c9d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2c9d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-118">Not Supported.</span></span>|
|<span data-ttu-id="d2c9d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2c9d-119">Application</span></span>|<span data-ttu-id="d2c9d-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2c9d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c9d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printerShares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2c9d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c9d-122">Request headers</span></span>
| <span data-ttu-id="d2c9d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d2c9d-123">Name</span></span>       | <span data-ttu-id="d2c9d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2c9d-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d2c9d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2c9d-125">Authorization</span></span> | <span data-ttu-id="d2c9d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2c9d-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="d2c9d-128">Content-type</span></span>  | <span data-ttu-id="d2c9d-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2c9d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c9d-131">Request body</span></span>
<span data-ttu-id="d2c9d-132">No corpo da solicitação, forneça os valores para campos [printerShare](../resources/printershare.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-132">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="d2c9d-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d2c9d-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d2c9d-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2c9d-135">Property</span></span>     | <span data-ttu-id="d2c9d-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2c9d-136">Type</span></span>        | <span data-ttu-id="d2c9d-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2c9d-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2c9d-138">impressora</span><span class="sxs-lookup"><span data-stu-id="d2c9d-138">printer</span></span>|<span data-ttu-id="d2c9d-139">String</span><span class="sxs-lookup"><span data-stu-id="d2c9d-139">String</span></span>|<span data-ttu-id="d2c9d-140">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-140">The printer that this printer share is related to.</span></span> <span data-ttu-id="d2c9d-141">Use a `printer@odata.bind` sintaxe, conforme mostrado no exemplo a seguir, para atualizar a impressora à qual este compartilhamento de impressora está associado.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-141">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|

><span data-ttu-id="d2c9d-142">**Observação:** Não há suporte para a atualização do nome de compartilhamento da impressora.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-142">**Note:** Updating the printer share name is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="d2c9d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c9d-143">Response</span></span>
<span data-ttu-id="d2c9d-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printerShare](../resources/printershare.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-144">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2c9d-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2c9d-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2c9d-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c9d-146">Request</span></span>
<span data-ttu-id="d2c9d-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printerShares/{id}
Content-type: application/json
Content-length: 109

{
  "name": "ShareName",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
##### <a name="response"></a><span data-ttu-id="d2c9d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c9d-148">Response</span></span>
<span data-ttu-id="d2c9d-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-149">The following is an example of the response.</span></span>
><span data-ttu-id="d2c9d-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2c9d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
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