---
title: assignLicense
description: Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96ececfce4800560b1f2ae625d12e67d10f3f325
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965772"
---
# <a name="assignlicense"></a><span data-ttu-id="8e059-104">assignLicense</span><span class="sxs-lookup"><span data-stu-id="8e059-104">assignLicense</span></span>
<span data-ttu-id="8e059-p102">Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="8e059-p102">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e059-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e059-107">Permissions</span></span>
<span data-ttu-id="8e059-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e059-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e059-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e059-110">Permission type</span></span>      | <span data-ttu-id="8e059-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e059-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e059-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e059-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8e059-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e059-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e059-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e059-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e059-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e059-115">Not supported.</span></span>    |
|<span data-ttu-id="8e059-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e059-116">Application</span></span> | <span data-ttu-id="8e059-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e059-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e059-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e059-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="8e059-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e059-119">Request headers</span></span>
| <span data-ttu-id="8e059-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e059-120">Header</span></span>       | <span data-ttu-id="8e059-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e059-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e059-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e059-122">Authorization</span></span>  | <span data-ttu-id="8e059-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e059-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8e059-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e059-125">Content-Type</span></span>  | <span data-ttu-id="8e059-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e059-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e059-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e059-127">Request body</span></span>
<span data-ttu-id="8e059-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e059-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e059-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8e059-129">Parameter</span></span>    | <span data-ttu-id="8e059-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e059-130">Type</span></span>   |<span data-ttu-id="8e059-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e059-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e059-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="8e059-132">addLicenses</span></span>|<span data-ttu-id="8e059-133">Coleção AssignedLicense</span><span class="sxs-lookup"><span data-stu-id="8e059-133">AssignedLicense collection</span></span>|<span data-ttu-id="8e059-p105">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar. Você pode desabilitar os planos associados a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="8e059-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="8e059-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="8e059-136">removeLicenses</span></span>|<span data-ttu-id="8e059-137">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="8e059-137">Guid collection</span></span>|<span data-ttu-id="8e059-138">Uma coleção de GUIDs que identifica as licenças a remover.</span><span class="sxs-lookup"><span data-stu-id="8e059-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="8e059-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e059-139">Response</span></span>

<span data-ttu-id="8e059-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e059-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e059-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e059-141">Example</span></span>
<span data-ttu-id="8e059-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8e059-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e059-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e059-143">Request</span></span>
<span data-ttu-id="8e059-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e059-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8e059-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e059-145">Response</span></span>
<span data-ttu-id="8e059-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e059-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
