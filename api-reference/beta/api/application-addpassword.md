---
title: 'Application: addpassword'
description: Adicione uma senha forte a um aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d067dfc1e0515d0a99848a9e94c910bf4a93f54
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936570"
---
# <a name="application-addpassword"></a><span data-ttu-id="97585-103">Application: addpassword</span><span class="sxs-lookup"><span data-stu-id="97585-103">application: addPassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97585-104">Adiciona uma senha forte a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="97585-104">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97585-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97585-105">Permissions</span></span>

<span data-ttu-id="97585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97585-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97585-108">Permission type</span></span>                        | <span data-ttu-id="97585-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97585-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97585-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97585-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97585-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97585-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="97585-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97585-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97585-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97585-113">Not supported.</span></span> |
| <span data-ttu-id="97585-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97585-114">Application</span></span>                            | <span data-ttu-id="97585-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97585-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97585-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97585-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="97585-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97585-117">Request headers</span></span>

| <span data-ttu-id="97585-118">Nome</span><span class="sxs-lookup"><span data-stu-id="97585-118">Name</span></span>           | <span data-ttu-id="97585-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="97585-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="97585-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="97585-120">Authorization</span></span>  | <span data-ttu-id="97585-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97585-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97585-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="97585-123">Content-type</span></span>   | <span data-ttu-id="97585-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97585-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97585-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97585-126">Request body</span></span>

<span data-ttu-id="97585-127">No corpo da solicitação, forneça um objeto `passwordCredential` opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="97585-127">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="97585-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97585-128">Property</span></span>     | <span data-ttu-id="97585-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="97585-129">Type</span></span>   |<span data-ttu-id="97585-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="97585-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97585-131">displayName</span><span class="sxs-lookup"><span data-stu-id="97585-131">displayName</span></span> | <span data-ttu-id="97585-132">String</span><span class="sxs-lookup"><span data-stu-id="97585-132">String</span></span> | <span data-ttu-id="97585-133">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="97585-133">Friendly name for the password.</span></span> <span data-ttu-id="97585-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97585-134">Optional.</span></span> |
| <span data-ttu-id="97585-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="97585-135">endDateTime</span></span> | <span data-ttu-id="97585-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97585-136">DateTimeOffset</span></span> | <span data-ttu-id="97585-137">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97585-137">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97585-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97585-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="97585-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97585-139">Optional.</span></span> |
| <span data-ttu-id="97585-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="97585-140">startDateTime</span></span> | <span data-ttu-id="97585-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97585-141">DateTimeOffset</span></span> | <span data-ttu-id="97585-142">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="97585-142">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="97585-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97585-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97585-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97585-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="97585-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97585-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="97585-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="97585-146">Response</span></span>

<span data-ttu-id="97585-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97585-147">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="97585-148">A propriedade **secretText** no objeto Response contém as senhas fortes geradas pelo Azure Active Directory com 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="97585-148">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="97585-149">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="97585-149">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="97585-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="97585-150">Examples</span></span>

<span data-ttu-id="97585-151">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="97585-151">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="97585-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97585-152">Request</span></span>

<span data-ttu-id="97585-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97585-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97585-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="97585-154">Response</span></span>

<span data-ttu-id="97585-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97585-155">The following is an example of the response.</span></span>

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
