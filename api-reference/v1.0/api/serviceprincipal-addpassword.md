---
title: 'servicePrincipal: addPassword'
description: Adicione uma senha forte a uma servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2da006952e418ab4ef4636a3aa7182ef1621ac10
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720907"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="27978-103">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="27978-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="27978-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27978-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27978-105">Adicione uma senha forte a um [objeto servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="27978-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27978-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="27978-106">Permissions</span></span>

<span data-ttu-id="27978-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27978-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27978-109">Permission type</span></span>                        | <span data-ttu-id="27978-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27978-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27978-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27978-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27978-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27978-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="27978-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27978-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27978-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27978-114">Not supported.</span></span> |
| <span data-ttu-id="27978-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27978-115">Application</span></span>                            | <span data-ttu-id="27978-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27978-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27978-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27978-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="27978-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27978-118">Request headers</span></span>

| <span data-ttu-id="27978-119">Nome</span><span class="sxs-lookup"><span data-stu-id="27978-119">Name</span></span>           | <span data-ttu-id="27978-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27978-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="27978-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="27978-121">Authorization</span></span>  | <span data-ttu-id="27978-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27978-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27978-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27978-124">Content-Type</span></span>   | <span data-ttu-id="27978-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27978-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27978-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27978-127">Request body</span></span>

<span data-ttu-id="27978-128">No corpo da solicitação, forneça um `passwordCredential` objeto opcional com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="27978-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="27978-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27978-129">Property</span></span>     | <span data-ttu-id="27978-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27978-130">Type</span></span>   |<span data-ttu-id="27978-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27978-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27978-132">displayName</span><span class="sxs-lookup"><span data-stu-id="27978-132">displayName</span></span> | <span data-ttu-id="27978-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27978-133">String</span></span> | <span data-ttu-id="27978-134">Nome amigável para a senha.</span><span class="sxs-lookup"><span data-stu-id="27978-134">Friendly name for the password.</span></span> <span data-ttu-id="27978-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27978-135">Optional.</span></span> |
| <span data-ttu-id="27978-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="27978-136">endDateTime</span></span> | <span data-ttu-id="27978-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27978-137">DateTimeOffset</span></span> | <span data-ttu-id="27978-138">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="27978-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="27978-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="27978-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="27978-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27978-140">Optional.</span></span> <span data-ttu-id="27978-141">O valor padrão é "startDateTime + 2 anos".</span><span class="sxs-lookup"><span data-stu-id="27978-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="27978-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="27978-142">startDateTime</span></span> | <span data-ttu-id="27978-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27978-143">DateTimeOffset</span></span> | <span data-ttu-id="27978-144">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="27978-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="27978-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="27978-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="27978-146">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="27978-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="27978-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27978-147">Optional.</span></span> <span data-ttu-id="27978-148">O valor padrão é "now".</span><span class="sxs-lookup"><span data-stu-id="27978-148">The default value is "now".</span></span>|

## <a name="response"></a><span data-ttu-id="27978-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="27978-149">Response</span></span>

<span data-ttu-id="27978-150">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27978-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="27978-151">A **propriedade secretText** no objeto de resposta contém as senhas fortes geradas pelo Azure Active Directory que têm de 16 a 64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="27978-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="27978-152">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="27978-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="27978-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27978-153">Examples</span></span>

<span data-ttu-id="27978-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="27978-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="27978-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27978-155">Request</span></span>

<span data-ttu-id="27978-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27978-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27978-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="27978-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="27978-158">C#</span><span class="sxs-lookup"><span data-stu-id="27978-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27978-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27978-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27978-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27978-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27978-161">Java</span><span class="sxs-lookup"><span data-stu-id="27978-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27978-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="27978-162">Response</span></span>

<span data-ttu-id="27978-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27978-163">The following is an example of the response.</span></span>

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

