---
title: 'servicePrincipal: addPassword'
description: Adicione uma senha forte a uma servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 518d7b696d214ead133bcf869381099034094359
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132010"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="f9f32-103">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="f9f32-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="f9f32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9f32-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9f32-105">Adicione uma senha forte a um [objeto servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="f9f32-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9f32-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9f32-106">Permissions</span></span>

<span data-ttu-id="f9f32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9f32-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9f32-109">Permission type</span></span>                        | <span data-ttu-id="f9f32-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9f32-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9f32-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9f32-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9f32-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9f32-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f9f32-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9f32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9f32-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f32-114">Not supported.</span></span> |
| <span data-ttu-id="f9f32-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9f32-115">Application</span></span>                            | <span data-ttu-id="f9f32-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f32-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9f32-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f32-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="f9f32-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f32-118">Request headers</span></span>

| <span data-ttu-id="f9f32-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f9f32-119">Name</span></span>           | <span data-ttu-id="f9f32-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9f32-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f9f32-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9f32-121">Authorization</span></span>  | <span data-ttu-id="f9f32-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f32-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9f32-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9f32-124">Content-Type</span></span>   | <span data-ttu-id="f9f32-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f32-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f32-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f32-127">Request body</span></span>

<span data-ttu-id="f9f32-128">No corpo da solicitação, forneça um `passwordCredential` objeto opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="f9f32-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="f9f32-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9f32-129">Property</span></span>     | <span data-ttu-id="f9f32-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9f32-130">Type</span></span>   |<span data-ttu-id="f9f32-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9f32-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9f32-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f9f32-132">displayName</span></span> | <span data-ttu-id="f9f32-133">String</span><span class="sxs-lookup"><span data-stu-id="f9f32-133">String</span></span> | <span data-ttu-id="f9f32-134">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="f9f32-134">Friendly name for the password.</span></span> <span data-ttu-id="f9f32-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9f32-135">Optional.</span></span> |
| <span data-ttu-id="f9f32-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f32-136">endDateTime</span></span> | <span data-ttu-id="f9f32-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f32-137">DateTimeOffset</span></span> | <span data-ttu-id="f9f32-138">A data e a hora em que a senha expira é representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f9f32-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f9f32-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f9f32-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f9f32-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9f32-140">Optional.</span></span> <span data-ttu-id="f9f32-141">O valor padrão é "startDateTime + 2 anos".</span><span class="sxs-lookup"><span data-stu-id="f9f32-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="f9f32-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f32-142">startDateTime</span></span> | <span data-ttu-id="f9f32-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f32-143">DateTimeOffset</span></span> | <span data-ttu-id="f9f32-144">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="f9f32-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="f9f32-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f9f32-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f9f32-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f9f32-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f9f32-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9f32-147">Optional.</span></span> <span data-ttu-id="f9f32-148">O valor padrão é "now".</span><span class="sxs-lookup"><span data-stu-id="f9f32-148">The default value is "now".</span></span>|

## <a name="response"></a><span data-ttu-id="f9f32-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f32-149">Response</span></span>

<span data-ttu-id="f9f32-150">Se bem-sucedido, este método retorna um código de resposta e `200 OK` um novo [objeto passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f32-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="f9f32-151">A **propriedade secretText** no objeto response contém as senhas fortes geradas pelo Azure Active Directory com 16 a 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f9f32-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="f9f32-152">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="f9f32-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="f9f32-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9f32-153">Examples</span></span>

<span data-ttu-id="f9f32-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f9f32-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f9f32-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f32-155">Request</span></span>

<span data-ttu-id="f9f32-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9f32-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9f32-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f32-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_addpassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f9f32-158">C#</span><span class="sxs-lookup"><span data-stu-id="f9f32-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9f32-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9f32-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9f32-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9f32-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9f32-161">Java</span><span class="sxs-lookup"><span data-stu-id="f9f32-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9f32-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f32-162">Response</span></span>

<span data-ttu-id="f9f32-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f32-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "customKeyIdentifier": null,
    "endDateTime": "2021-09-09T19:50:29.3086381Z",
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "startDateTime": "2019-09-09T19:50:29.3086381Z",
    "secretText": "[6gyXA5S20@MN+WRXAJ]I-TO7g1:h2P8",
    "hint": "[6g",
    "displayName": "Password friendly name"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

