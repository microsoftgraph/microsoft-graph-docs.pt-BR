---
title: 'servicePrincipalName: addpassword'
description: Adicione uma senha forte a um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 11a8d6e6a54941e6ecee10878c01ed0e5f5e91da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453524"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="84ddd-103">servicePrincipalName: addpassword</span><span class="sxs-lookup"><span data-stu-id="84ddd-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="84ddd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84ddd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84ddd-105">Adicione uma senha forte a um objeto de [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="84ddd-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84ddd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84ddd-106">Permissions</span></span>

<span data-ttu-id="84ddd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84ddd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84ddd-109">Permission type</span></span>                        | <span data-ttu-id="84ddd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84ddd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84ddd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84ddd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="84ddd-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84ddd-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="84ddd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84ddd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84ddd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84ddd-114">Not supported.</span></span> |
| <span data-ttu-id="84ddd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84ddd-115">Application</span></span>                            | <span data-ttu-id="84ddd-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ddd-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84ddd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84ddd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="84ddd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84ddd-118">Request headers</span></span>

| <span data-ttu-id="84ddd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="84ddd-119">Name</span></span>           | <span data-ttu-id="84ddd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ddd-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="84ddd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="84ddd-121">Authorization</span></span>  | <span data-ttu-id="84ddd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84ddd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="84ddd-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="84ddd-124">Content-type</span></span>   | <span data-ttu-id="84ddd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84ddd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ddd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84ddd-127">Request body</span></span>

<span data-ttu-id="84ddd-128">No corpo da solicitação, forneça um objeto `passwordCredential` opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="84ddd-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="84ddd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84ddd-129">Property</span></span>     | <span data-ttu-id="84ddd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="84ddd-130">Type</span></span>   |<span data-ttu-id="84ddd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ddd-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84ddd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="84ddd-132">displayName</span></span> | <span data-ttu-id="84ddd-133">String</span><span class="sxs-lookup"><span data-stu-id="84ddd-133">String</span></span> | <span data-ttu-id="84ddd-134">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="84ddd-134">Friendly name for the password.</span></span> <span data-ttu-id="84ddd-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="84ddd-135">Optional.</span></span> |
| <span data-ttu-id="84ddd-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="84ddd-136">endDateTime</span></span> | <span data-ttu-id="84ddd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84ddd-137">DateTimeOffset</span></span> | <span data-ttu-id="84ddd-138">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="84ddd-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="84ddd-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="84ddd-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="84ddd-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="84ddd-140">Optional.</span></span> |
| <span data-ttu-id="84ddd-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="84ddd-141">startDateTime</span></span> | <span data-ttu-id="84ddd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84ddd-142">DateTimeOffset</span></span> | <span data-ttu-id="84ddd-143">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="84ddd-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="84ddd-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="84ddd-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="84ddd-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="84ddd-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="84ddd-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="84ddd-146">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="84ddd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="84ddd-147">Response</span></span>

<span data-ttu-id="84ddd-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84ddd-148">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="84ddd-149">A propriedade **secretText** no objeto Response contém as senhas fortes geradas pelo Azure Active Directory com 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="84ddd-149">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="84ddd-150">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="84ddd-150">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="84ddd-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="84ddd-151">Examples</span></span>

<span data-ttu-id="84ddd-152">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="84ddd-152">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="84ddd-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84ddd-153">Request</span></span>

<span data-ttu-id="84ddd-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84ddd-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84ddd-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="84ddd-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_addpassword"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="84ddd-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84ddd-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84ddd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="84ddd-157">Response</span></span>

<span data-ttu-id="84ddd-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84ddd-158">The following is an example of the response.</span></span>

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
