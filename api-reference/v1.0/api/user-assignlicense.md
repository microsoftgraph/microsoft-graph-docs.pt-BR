---
title: assignLicense
description: Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8a6a6cca2374df1870214083cfa46b9f8c5d8211
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721590"
---
# <a name="user-assignlicense"></a><span data-ttu-id="c3f24-104">usuário: assignLicense</span><span class="sxs-lookup"><span data-stu-id="c3f24-104">user: assignLicense</span></span>

<span data-ttu-id="c3f24-p102">Namespace: microsoft.graph Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3f24-p102">Namespace: microsoft.graph Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f24-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3f24-107">Permissions</span></span>
<span data-ttu-id="c3f24-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3f24-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3f24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3f24-110">Permission type</span></span>      | <span data-ttu-id="c3f24-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3f24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3f24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3f24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c3f24-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f24-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3f24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3f24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3f24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3f24-115">Not supported.</span></span>    |
|<span data-ttu-id="c3f24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3f24-116">Application</span></span> | <span data-ttu-id="c3f24-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f24-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3f24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f24-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="c3f24-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f24-119">Request headers</span></span>
| <span data-ttu-id="c3f24-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3f24-120">Header</span></span>       | <span data-ttu-id="c3f24-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c3f24-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3f24-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3f24-122">Authorization</span></span>  | <span data-ttu-id="c3f24-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3f24-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c3f24-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3f24-125">Content-Type</span></span>  | <span data-ttu-id="c3f24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3f24-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3f24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f24-127">Request body</span></span>
<span data-ttu-id="c3f24-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3f24-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3f24-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c3f24-129">Parameter</span></span>    | <span data-ttu-id="c3f24-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3f24-130">Type</span></span>   |<span data-ttu-id="c3f24-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f24-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3f24-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="c3f24-132">addLicenses</span></span>|<span data-ttu-id="c3f24-133">Coleção assignedLicense</span><span class="sxs-lookup"><span data-stu-id="c3f24-133">AssignedLicense collection</span></span>|<span data-ttu-id="c3f24-p105">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar. Você pode desabilitar os planos associados a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="c3f24-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="c3f24-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="c3f24-136">removeLicenses</span></span>|<span data-ttu-id="c3f24-137">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="c3f24-137">Guid collection</span></span>|<span data-ttu-id="c3f24-138">Uma coleção de GUIDs que identifica as licenças a remover.</span><span class="sxs-lookup"><span data-stu-id="c3f24-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="c3f24-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f24-139">Response</span></span>

<span data-ttu-id="c3f24-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f24-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3f24-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3f24-141">Example</span></span>
<span data-ttu-id="c3f24-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c3f24-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c3f24-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f24-143">Request</span></span>
<span data-ttu-id="c3f24-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3f24-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3f24-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f24-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "guid"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```
# <a name="c"></a>[<span data-ttu-id="c3f24-146">C#</span><span class="sxs-lookup"><span data-stu-id="c3f24-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3f24-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3f24-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3f24-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3f24-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3f24-149">Java</span><span class="sxs-lookup"><span data-stu-id="c3f24-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c3f24-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f24-150">Response</span></span>
<span data-ttu-id="c3f24-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3f24-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "0118A350-71FC-4EC3-8F0C-6A1CB8867561"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-02T12:13:14Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

