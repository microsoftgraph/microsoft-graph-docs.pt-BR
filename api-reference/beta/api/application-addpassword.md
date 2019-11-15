---
title: 'Application: addpassword'
description: Adicionar uma senha forte a um aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3584d7e0b5bcf7d73838da08f502d681f4f4276c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995588"
---
# <a name="application-addpassword"></a><span data-ttu-id="90a3b-103">Application: addpassword</span><span class="sxs-lookup"><span data-stu-id="90a3b-103">application: addPassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90a3b-104">Adiciona uma senha forte a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="90a3b-104">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="90a3b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="90a3b-105">Permissions</span></span>

<span data-ttu-id="90a3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90a3b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90a3b-108">Permission type</span></span>                        | <span data-ttu-id="90a3b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90a3b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90a3b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90a3b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="90a3b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90a3b-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="90a3b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90a3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90a3b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90a3b-113">Not supported.</span></span> |
| <span data-ttu-id="90a3b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90a3b-114">Application</span></span>                            | <span data-ttu-id="90a3b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90a3b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90a3b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90a3b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="90a3b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90a3b-117">Request headers</span></span>

| <span data-ttu-id="90a3b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="90a3b-118">Name</span></span>           | <span data-ttu-id="90a3b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="90a3b-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="90a3b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="90a3b-120">Authorization</span></span>  | <span data-ttu-id="90a3b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90a3b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90a3b-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="90a3b-123">Content-type</span></span>   | <span data-ttu-id="90a3b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90a3b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90a3b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90a3b-126">Request body</span></span>

<span data-ttu-id="90a3b-127">No corpo da solicitação, forneça um objeto `passwordCredential` opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="90a3b-127">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="90a3b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90a3b-128">Property</span></span>     | <span data-ttu-id="90a3b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="90a3b-129">Type</span></span>   |<span data-ttu-id="90a3b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="90a3b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="90a3b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="90a3b-131">displayName</span></span> | <span data-ttu-id="90a3b-132">String</span><span class="sxs-lookup"><span data-stu-id="90a3b-132">String</span></span> | <span data-ttu-id="90a3b-133">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="90a3b-133">Friendly name for the password.</span></span> <span data-ttu-id="90a3b-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90a3b-134">Optional.</span></span> |
| <span data-ttu-id="90a3b-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="90a3b-135">endDateTime</span></span> | <span data-ttu-id="90a3b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a3b-136">DateTimeOffset</span></span> | <span data-ttu-id="90a3b-137">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90a3b-137">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a3b-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="90a3b-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="90a3b-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90a3b-139">Optional.</span></span> |
| <span data-ttu-id="90a3b-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="90a3b-140">startDateTime</span></span> | <span data-ttu-id="90a3b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a3b-141">DateTimeOffset</span></span> | <span data-ttu-id="90a3b-142">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="90a3b-142">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="90a3b-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90a3b-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a3b-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="90a3b-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="90a3b-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90a3b-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="90a3b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="90a3b-146">Response</span></span>

<span data-ttu-id="90a3b-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90a3b-147">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="90a3b-148">A propriedade **secretText** no objeto Response contém as senhas fortes geradas pelo Azure Active Directory com 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="90a3b-148">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="90a3b-149">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="90a3b-149">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="90a3b-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90a3b-150">Examples</span></span>

<span data-ttu-id="90a3b-151">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="90a3b-151">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="90a3b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90a3b-152">Request</span></span>

<span data-ttu-id="90a3b-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90a3b-153">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90a3b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="90a3b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addpassword"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90a3b-155">C#</span><span class="sxs-lookup"><span data-stu-id="90a3b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90a3b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90a3b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90a3b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90a3b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90a3b-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="90a3b-158">Response</span></span>

<span data-ttu-id="90a3b-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90a3b-159">The following is an example of the response.</span></span>

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
  "description": "application: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
