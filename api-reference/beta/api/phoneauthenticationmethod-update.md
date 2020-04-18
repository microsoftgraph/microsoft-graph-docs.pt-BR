---
title: Atualizar phoneAuthenticationMethod
description: Atualize o número de telefone associado ao objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c1a408fddaa53de9d6741cb4cc86a948db9ccb44
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557786"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="d99af-103">Atualizar phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d99af-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="d99af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d99af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d99af-105">Atualize o número de telefone associado a um [método de autenticação de telefone](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="d99af-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="d99af-106">Não é possível alterar o tipo de um telefone.</span><span class="sxs-lookup"><span data-stu-id="d99af-106">You can't change a phone's type.</span></span> <span data-ttu-id="d99af-107">Para alterar o tipo de um telefone, adicione um novo número do tipo desejado e exclua o objeto com o tipo original.</span><span class="sxs-lookup"><span data-stu-id="d99af-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="d99af-108">Se um usuário estiver habilitado por política para usar o SMS para entrar e o `mobile` número for alterado, o sistema tentará registrar o número para uso nesse sistema.</span><span class="sxs-lookup"><span data-stu-id="d99af-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="d99af-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d99af-109">Permissions</span></span>

<span data-ttu-id="d99af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d99af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d99af-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d99af-112">Permission type</span></span>                        | <span data-ttu-id="d99af-113">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d99af-113">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="d99af-114">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d99af-114">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d99af-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d99af-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d99af-116">UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d99af-116">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="d99af-117">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d99af-117">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d99af-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d99af-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d99af-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d99af-119">Not supported.</span></span> | <span data-ttu-id="d99af-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d99af-120">Not supported.</span></span> |
| <span data-ttu-id="d99af-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d99af-121">Application</span></span>                            | <span data-ttu-id="d99af-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d99af-122">Not supported.</span></span> | <span data-ttu-id="d99af-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d99af-123">Not supported.</span></span> |

<span data-ttu-id="d99af-124">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="d99af-124">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d99af-125">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d99af-125">Global admin</span></span>
* <span data-ttu-id="d99af-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="d99af-126">Privileged authentication admin</span></span>
* <span data-ttu-id="d99af-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="d99af-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d99af-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d99af-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d99af-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d99af-129">Request headers</span></span>

| <span data-ttu-id="d99af-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d99af-130">Name</span></span>       | <span data-ttu-id="d99af-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d99af-131">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d99af-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d99af-132">Authorization</span></span> | <span data-ttu-id="d99af-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d99af-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d99af-135">Content-type</span><span class="sxs-lookup"><span data-stu-id="d99af-135">Content-type</span></span>  | <span data-ttu-id="d99af-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d99af-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d99af-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d99af-138">Request body</span></span>

<span data-ttu-id="d99af-139">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d99af-139">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d99af-140">As propriedades existentes que não estão incluídas no corpo da solicitação serão recalculadas com base nas alterações de outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d99af-140">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="d99af-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d99af-141">Property</span></span>     | <span data-ttu-id="d99af-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="d99af-142">Type</span></span>        | <span data-ttu-id="d99af-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="d99af-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d99af-144">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d99af-144">phoneNumber</span></span>|<span data-ttu-id="d99af-145">String</span><span class="sxs-lookup"><span data-stu-id="d99af-145">String</span></span>|<span data-ttu-id="d99af-146">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="d99af-146">The phone number to text or call for authentication.</span></span> <span data-ttu-id="d99af-147">Os números de telefone usam o formato\<"+\> \<ramal\>\>de\<código de país x", com a extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="d99af-147">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="d99af-148">Por exemplo, + 1 5555551234 ou + 1 5555551234x123 são válidas.</span><span class="sxs-lookup"><span data-stu-id="d99af-148">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="d99af-149">Os números são rejeitados ao criar/atualizar se não coincidem com o formato necessário.</span><span class="sxs-lookup"><span data-stu-id="d99af-149">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="d99af-150">PhoneType</span><span class="sxs-lookup"><span data-stu-id="d99af-150">phoneType</span></span>|<span data-ttu-id="d99af-151">string</span><span class="sxs-lookup"><span data-stu-id="d99af-151">string</span></span>| <span data-ttu-id="d99af-152">Os valores possíveis são `mobile`: `alternateMobile`,, `office`ou.</span><span class="sxs-lookup"><span data-stu-id="d99af-152">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="d99af-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d99af-153">Response</span></span>

<span data-ttu-id="d99af-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d99af-154">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d99af-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d99af-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d99af-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d99af-156">Request</span></span>

<span data-ttu-id="d99af-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d99af-157">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```

### <a name="response"></a><span data-ttu-id="d99af-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d99af-158">Response</span></span>

<span data-ttu-id="d99af-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d99af-159">The following is an example of the response.</span></span>

> <span data-ttu-id="d99af-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d99af-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
