---
title: 'Application: addpassword'
description: Adicionar uma senha forte a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84270f5be2d647c5b1ab884802ef3b363e81eaff
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107245"
---
# <a name="application-addpassword"></a><span data-ttu-id="16f4f-103">Application: addpassword</span><span class="sxs-lookup"><span data-stu-id="16f4f-103">application: addPassword</span></span>

<span data-ttu-id="16f4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16f4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16f4f-105">Adiciona uma senha forte a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="16f4f-105">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16f4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="16f4f-106">Permissions</span></span>

<span data-ttu-id="16f4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16f4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16f4f-109">Permission type</span></span>                        | <span data-ttu-id="16f4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16f4f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="16f4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16f4f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16f4f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16f4f-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="16f4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16f4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16f4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16f4f-114">Not supported.</span></span> |
| <span data-ttu-id="16f4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16f4f-115">Application</span></span>                            | <span data-ttu-id="16f4f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16f4f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16f4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16f4f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="16f4f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16f4f-118">Request headers</span></span>

| <span data-ttu-id="16f4f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="16f4f-119">Name</span></span>           | <span data-ttu-id="16f4f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="16f4f-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="16f4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="16f4f-121">Authorization</span></span>  | <span data-ttu-id="16f4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16f4f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16f4f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="16f4f-124">Content-type</span></span>   | <span data-ttu-id="16f4f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16f4f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16f4f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16f4f-127">Request body</span></span>

<span data-ttu-id="16f4f-128">No corpo da solicitação, forneça um objeto `passwordCredential` opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="16f4f-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="16f4f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16f4f-129">Property</span></span>     | <span data-ttu-id="16f4f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16f4f-130">Type</span></span>   |<span data-ttu-id="16f4f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16f4f-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16f4f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="16f4f-132">displayName</span></span> | <span data-ttu-id="16f4f-133">String</span><span class="sxs-lookup"><span data-stu-id="16f4f-133">String</span></span> | <span data-ttu-id="16f4f-134">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="16f4f-134">Friendly name for the password.</span></span> <span data-ttu-id="16f4f-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16f4f-135">Optional.</span></span> |
| <span data-ttu-id="16f4f-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="16f4f-136">endDateTime</span></span> | <span data-ttu-id="16f4f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16f4f-137">DateTimeOffset</span></span> | <span data-ttu-id="16f4f-138">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="16f4f-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="16f4f-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="16f4f-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="16f4f-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16f4f-140">Optional.</span></span> |
| <span data-ttu-id="16f4f-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="16f4f-141">startDateTime</span></span> | <span data-ttu-id="16f4f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16f4f-142">DateTimeOffset</span></span> | <span data-ttu-id="16f4f-143">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="16f4f-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="16f4f-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="16f4f-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="16f4f-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="16f4f-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="16f4f-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16f4f-146">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="16f4f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f4f-147">Response</span></span>

<span data-ttu-id="16f4f-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16f4f-148">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="16f4f-149">A propriedade **secretText** no objeto Response contém as senhas fortes geradas pelo Azure Active Directory com 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="16f4f-149">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="16f4f-150">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="16f4f-150">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="16f4f-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16f4f-151">Examples</span></span>

<span data-ttu-id="16f4f-152">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="16f4f-152">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="16f4f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16f4f-153">Request</span></span>

<span data-ttu-id="16f4f-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16f4f-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16f4f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="16f4f-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="16f4f-156">C#</span><span class="sxs-lookup"><span data-stu-id="16f4f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16f4f-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16f4f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16f4f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16f4f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16f4f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f4f-159">Response</span></span>

<span data-ttu-id="16f4f-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16f4f-160">The following is an example of the response.</span></span>

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
