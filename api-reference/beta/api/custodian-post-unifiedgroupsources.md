---
title: Criar unifiedGroupSource
description: Crie um novo objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 61e7ff3aef7c4a94b0a0efcbc0f012b7eda0b604
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872545"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="b2580-103">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="b2580-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="b2580-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2580-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2580-105">Crie um novo [objeto unifiedGroupSource.](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="b2580-105">Create a new [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2580-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2580-106">Permissions</span></span>

<span data-ttu-id="b2580-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2580-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2580-109">Permission type</span></span>|<span data-ttu-id="b2580-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2580-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2580-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2580-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2580-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="b2580-112">User.Read</span></span>|
|<span data-ttu-id="b2580-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2580-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2580-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2580-114">Not supported.</span></span>|
|<span data-ttu-id="b2580-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2580-115">Application</span></span>|<span data-ttu-id="b2580-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2580-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2580-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2580-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="b2580-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2580-118">Request headers</span></span>

|<span data-ttu-id="b2580-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b2580-119">Name</span></span>|<span data-ttu-id="b2580-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2580-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b2580-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2580-121">Authorization</span></span>|<span data-ttu-id="b2580-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2580-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b2580-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2580-124">Content-Type</span></span>|<span data-ttu-id="b2580-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2580-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2580-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2580-127">Request body</span></span>

<span data-ttu-id="b2580-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedGroupSource.](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="b2580-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="b2580-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unifiedGroupSource](../resources/unifiedgroupsource.md).</span><span class="sxs-lookup"><span data-stu-id="b2580-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/unifiedgroupsource.md).</span></span>

|<span data-ttu-id="b2580-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2580-130">Property</span></span>|<span data-ttu-id="b2580-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2580-131">Type</span></span>|<span data-ttu-id="b2580-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2580-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2580-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="b2580-133">includedSources</span></span>|<span data-ttu-id="b2580-134">sourceType</span><span class="sxs-lookup"><span data-stu-id="b2580-134">sourceType</span></span>|<span data-ttu-id="b2580-135">Especifica quais fontes estão incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="b2580-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="b2580-136">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="b2580-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="b2580-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="b2580-137">group@odata.bind</span></span>|<span data-ttu-id="b2580-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2580-138">String</span></span>|<span data-ttu-id="b2580-139">ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="b2580-139">ID of the group.</span></span> <span data-ttu-id="b2580-140">Para obter a ID do grupo, use a operação [listar grupos.](../api/group-list.md)</span><span class="sxs-lookup"><span data-stu-id="b2580-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="b2580-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2580-141">Response</span></span>

<span data-ttu-id="b2580-142">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [unifiedGroupSource](../resources/unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2580-142">If successful, this method returns a `201 Created` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2580-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b2580-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2580-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2580-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b2580-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2580-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```
# <a name="c"></a>[<span data-ttu-id="b2580-146">C#</span><span class="sxs-lookup"><span data-stu-id="b2580-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2580-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2580-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2580-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2580-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedgroupsource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2580-149">Java</span><span class="sxs-lookup"><span data-stu-id="b2580-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2580-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2580-150">Response</span></span>

<span data-ttu-id="b2580-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2580-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site",
  "id": "14202dd90a1f4ccc84929586326c7104",
  "displayName": "SFA Videos",
  "createdDateTime": "2020-03-13T22:38:00.8985662Z",
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Megan Bowen"
      }
  }
}
```
