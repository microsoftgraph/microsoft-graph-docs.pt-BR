---
title: 'servicePrincipalName: addpassword'
description: Adicione uma senha forte a um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fcf5ba9d2e923b4b95c42e9ba22b0329c0e9b831
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289911"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="d766c-103">servicePrincipalName: addpassword</span><span class="sxs-lookup"><span data-stu-id="d766c-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="d766c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d766c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d766c-105">Adicione uma senha forte a um objeto de [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="d766c-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d766c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d766c-106">Permissions</span></span>

<span data-ttu-id="d766c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d766c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d766c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d766c-109">Permission type</span></span>                        | <span data-ttu-id="d766c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d766c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d766c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d766c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d766c-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="d766c-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d766c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d766c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d766c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d766c-114">Not supported.</span></span> |
| <span data-ttu-id="d766c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d766c-115">Application</span></span>                            | <span data-ttu-id="d766c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d766c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d766c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d766c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="d766c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d766c-118">Request headers</span></span>

| <span data-ttu-id="d766c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d766c-119">Name</span></span>           | <span data-ttu-id="d766c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d766c-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d766c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d766c-121">Authorization</span></span>  | <span data-ttu-id="d766c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d766c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d766c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d766c-124">Content-Type</span></span>   | <span data-ttu-id="d766c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d766c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d766c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d766c-127">Request body</span></span>

<span data-ttu-id="d766c-128">No corpo da solicitação, forneça um `passwordCredential` objeto opcional com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="d766c-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="d766c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d766c-129">Property</span></span>     | <span data-ttu-id="d766c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d766c-130">Type</span></span>   |<span data-ttu-id="d766c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d766c-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d766c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d766c-132">displayName</span></span> | <span data-ttu-id="d766c-133">String</span><span class="sxs-lookup"><span data-stu-id="d766c-133">String</span></span> | <span data-ttu-id="d766c-134">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="d766c-134">Friendly name for the password.</span></span> <span data-ttu-id="d766c-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d766c-135">Optional.</span></span> |
| <span data-ttu-id="d766c-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d766c-136">endDateTime</span></span> | <span data-ttu-id="d766c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d766c-137">DateTimeOffset</span></span> | <span data-ttu-id="d766c-138">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d766c-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d766c-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d766c-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d766c-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d766c-140">Optional.</span></span> <span data-ttu-id="d766c-141">O valor padrão é "startDatetime + 2 anos".</span><span class="sxs-lookup"><span data-stu-id="d766c-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="d766c-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d766c-142">startDateTime</span></span> | <span data-ttu-id="d766c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d766c-143">DateTimeOffset</span></span> | <span data-ttu-id="d766c-144">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="d766c-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="d766c-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d766c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d766c-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d766c-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d766c-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d766c-147">Optional.</span></span> <span data-ttu-id="d766c-148">O valor padrão é "Now".</span><span class="sxs-lookup"><span data-stu-id="d766c-148">The default value is "now".</span></span>|

## <a name="response"></a><span data-ttu-id="d766c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d766c-149">Response</span></span>

<span data-ttu-id="d766c-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d766c-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="d766c-151">A propriedade **secretText** no objeto Response contém as senhas fortes geradas pelo Azure Active Directory com 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="d766c-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="d766c-152">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="d766c-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="d766c-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d766c-153">Examples</span></span>

<span data-ttu-id="d766c-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d766c-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d766c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d766c-155">Request</span></span>

<span data-ttu-id="d766c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d766c-156">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d766c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d766c-157">Response</span></span>

<span data-ttu-id="d766c-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d766c-158">The following is an example of the response.</span></span>

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
