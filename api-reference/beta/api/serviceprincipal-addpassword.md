---
title: 'servicePrincipal: addPassword'
description: Adicione uma senha forte a uma servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 167ad25cc11dc7fe730ad863af95f2303d7ab178
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131961"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="37a61-103">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="37a61-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="37a61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a61-105">Adicione uma senha forte a um [objeto servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="37a61-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37a61-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37a61-106">Permissions</span></span>

<span data-ttu-id="37a61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37a61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37a61-109">Permission type</span></span>                        | <span data-ttu-id="37a61-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37a61-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37a61-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37a61-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37a61-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37a61-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="37a61-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37a61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a61-114">Not supported.</span></span> |
| <span data-ttu-id="37a61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37a61-115">Application</span></span>                            | <span data-ttu-id="37a61-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a61-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37a61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37a61-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="37a61-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37a61-118">Request headers</span></span>

| <span data-ttu-id="37a61-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37a61-119">Name</span></span>           | <span data-ttu-id="37a61-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a61-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="37a61-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37a61-121">Authorization</span></span>  | <span data-ttu-id="37a61-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a61-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37a61-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37a61-124">Content-Type</span></span>   | <span data-ttu-id="37a61-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a61-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a61-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37a61-127">Request body</span></span>

<span data-ttu-id="37a61-128">No corpo da solicitação, forneça um `passwordCredential` objeto opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="37a61-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="37a61-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37a61-129">Property</span></span>     | <span data-ttu-id="37a61-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a61-130">Type</span></span>   |<span data-ttu-id="37a61-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a61-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="37a61-132">displayName</span><span class="sxs-lookup"><span data-stu-id="37a61-132">displayName</span></span> | <span data-ttu-id="37a61-133">String</span><span class="sxs-lookup"><span data-stu-id="37a61-133">String</span></span> | <span data-ttu-id="37a61-134">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="37a61-134">Friendly name for the password.</span></span> <span data-ttu-id="37a61-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a61-135">Optional.</span></span> |
| <span data-ttu-id="37a61-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="37a61-136">endDateTime</span></span> | <span data-ttu-id="37a61-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37a61-137">DateTimeOffset</span></span> | <span data-ttu-id="37a61-138">A data e a hora em que a senha expira é representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="37a61-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37a61-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="37a61-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="37a61-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a61-140">Optional.</span></span> <span data-ttu-id="37a61-141">O valor padrão é "startDateTime + 2 anos".</span><span class="sxs-lookup"><span data-stu-id="37a61-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="37a61-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="37a61-142">startDateTime</span></span> | <span data-ttu-id="37a61-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37a61-143">DateTimeOffset</span></span> | <span data-ttu-id="37a61-144">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="37a61-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="37a61-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="37a61-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37a61-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="37a61-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="37a61-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a61-147">Optional.</span></span> <span data-ttu-id="37a61-148">O valor padrão é "now".</span><span class="sxs-lookup"><span data-stu-id="37a61-148">The default value is "now".</span></span> |

## <a name="response"></a><span data-ttu-id="37a61-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a61-149">Response</span></span>

<span data-ttu-id="37a61-150">Se bem-sucedido, este método retorna um código de resposta e `200 OK` um novo [objeto passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37a61-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="37a61-151">A **propriedade secretText** no objeto response contém as senhas fortes geradas pelo Azure Active Directory com 16 a 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="37a61-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="37a61-152">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="37a61-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="37a61-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37a61-153">Examples</span></span>

<span data-ttu-id="37a61-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="37a61-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="37a61-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a61-155">Request</span></span>

<span data-ttu-id="37a61-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a61-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37a61-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a61-157">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="37a61-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a61-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37a61-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a61-159">Response</span></span>

<span data-ttu-id="37a61-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37a61-160">The following is an example of the response.</span></span>

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



