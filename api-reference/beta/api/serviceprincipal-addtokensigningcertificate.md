---
title: 'servicePrincipal: addTokenSigningCertificate'
description: Adicione um certificado de assinatura a um servicePrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 01aded24ecce1b15c7bb56b9c5054f887098dc38
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787223"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a><span data-ttu-id="3aaf5-103">servicePrincipal: addTokenSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="3aaf5-103">servicePrincipal: addTokenSigningCertificate</span></span>

<span data-ttu-id="3aaf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aaf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aaf5-105">Cria um certificado de assinatura auto-assinado e retorna um [selfSignedCertificate](../resources/selfsignedcertificate.md), que é a parte pública do certificado gerado.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-105">Creates a self-signed signing certificate and returns a [selfSignedCertificate](../resources/selfsignedcertificate.md), which is the public part of the generated certificate.</span></span> <span data-ttu-id="3aaf5-106">O certificado de assinatura auto-assinado é composto por esses recursos: a chave privada ([keyCredential](../resources/keycredential.md) com uso = 'Sign'), a chave pública ([keyCredential](../resources/keycredential.md) com uso = 'verify') e [a passwordCredential](../resources/passwordcredential.md).</span><span class="sxs-lookup"><span data-stu-id="3aaf5-106">The self-signed signing certificate is composed of these resources: the private key ([keyCredential](../resources/keycredential.md) with usage = 'Sign'), the public key ([keyCredential](../resources/keycredential.md) with usage = 'verify'), and the [passwordCredential](../resources/passwordcredential.md).</span></span> <span data-ttu-id="3aaf5-107">Todos os recursos criados têm o **mesmo customKeyIdentifier**.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-107">All the created resources have the same **customKeyIdentifier**.</span></span>

<span data-ttu-id="3aaf5-108">A **senhaCredential** é usada para abrir a chave pfx/privada.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-108">The **passwordCredential** is used to open the pfx/private key.</span></span> <span data-ttu-id="3aaf5-109">Além disso, ele está associado ao privateKey ter a mesma **keyId**.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-109">Also, it's associated with the privateKey having the same **keyId**.</span></span> <span data-ttu-id="3aaf5-110">O assunto do certificado é um valor constante.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-110">The subject of the certificate is a constant value.</span></span> <span data-ttu-id="3aaf5-111">Ele não será afetado pelo **displayName opcional** fornecido na chamada POST.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-111">It won't be affected by the optional **displayName** provided in the POST call.</span></span> <span data-ttu-id="3aaf5-112">O **startDateTime** é definido para o mesmo horário em que o certificado é criado usando a ação.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-112">The **startDateTime** is set to the same time the certificate is created using the action.</span></span> <span data-ttu-id="3aaf5-113">O **endDateTime** pode ter até três anos após a criação do certificado.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-113">The **endDateTime** can be up to three years after the certificate is created.</span></span>

## <a name="permissions"></a><span data-ttu-id="3aaf5-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="3aaf5-114">Permissions</span></span>

|<span data-ttu-id="3aaf5-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aaf5-115">Permission type</span></span>      | <span data-ttu-id="3aaf5-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aaf5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aaf5-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aaf5-117">Delegated (work or school account)</span></span> | <span data-ttu-id="3aaf5-118">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aaf5-118">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3aaf5-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aaf5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aaf5-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-120">None.</span></span>    |
|<span data-ttu-id="3aaf5-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aaf5-121">Application</span></span> | <span data-ttu-id="3aaf5-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aaf5-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3aaf5-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aaf5-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a><span data-ttu-id="3aaf5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaf5-124">Request body</span></span>

<span data-ttu-id="3aaf5-125">No corpo da solicitação, forneça as seguintes propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-125">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="3aaf5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aaf5-126">Property</span></span>     | <span data-ttu-id="3aaf5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aaf5-127">Type</span></span>   |<span data-ttu-id="3aaf5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aaf5-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3aaf5-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3aaf5-129">displayName</span></span> | <span data-ttu-id="3aaf5-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3aaf5-130">string</span></span> | <span data-ttu-id="3aaf5-131">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-131">Friendly name for the key.</span></span>  <span data-ttu-id="3aaf5-132">Ele deve começar com `CN=` .</span><span class="sxs-lookup"><span data-stu-id="3aaf5-132">It must start with `CN=`.</span></span>|
| <span data-ttu-id="3aaf5-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3aaf5-133">endDateTime</span></span> | <span data-ttu-id="3aaf5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aaf5-134">DateTimeOffset</span></span> |<span data-ttu-id="3aaf5-135">A data e a hora em que a credencial expira.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-135">The date and time when the credential expires.</span></span> <span data-ttu-id="3aaf5-136">Pode ser até 3 anos a partir da data em que o certificado é criado.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-136">It can be up to 3 years from the date the certificate is created.</span></span> <span data-ttu-id="3aaf5-137">Se não for fornecido, o padrão será de três anos a partir do momento da criação.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-137">If not supplied, the default is three years from the time of creation.</span></span> <span data-ttu-id="3aaf5-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3aaf5-139">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z' .</span><span class="sxs-lookup"><span data-stu-id="3aaf5-139">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z' .</span></span>|

## <a name="response"></a><span data-ttu-id="3aaf5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaf5-140">Response</span></span>

<span data-ttu-id="3aaf5-141">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [selfSignedCertificate](../resources/selfsignedcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-141">If successful, this method returns a `200 OK` response code and a new [selfSignedCertificate](../resources/selfsignedcertificate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3aaf5-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3aaf5-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3aaf5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaf5-143">Request</span></span>

<span data-ttu-id="3aaf5-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3aaf5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aaf5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```
# <a name="c"></a>[<span data-ttu-id="3aaf5-146">C#</span><span class="sxs-lookup"><span data-stu-id="3aaf5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addtokensigningcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aaf5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aaf5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addtokensigningcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aaf5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aaf5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addtokensigningcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aaf5-149">Java</span><span class="sxs-lookup"><span data-stu-id="3aaf5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addtokensigningcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3aaf5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaf5-150">Response</span></span>

<span data-ttu-id="3aaf5-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3aaf5-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.selfSignedCertificate"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "2iD8ppbE+D6Kmu1ZvjM2jtQh88E=",
  "displayName": "CN=customDisplayName",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICuDCCAaCgAwIBAgIIYXJsNtL4oUMwDQYJKoZIhvcNAQEL...StP8s/w==",
  "keyId": "93bc223f-7235-4b9c-beea-d66847531c49",
  "startDateTime": "2021-05-05T18:38:51.8100763Z",
  "thumbprint": "DA20FCA696C4F83E8A9AED59BE33368ED421F3C1",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-01-15 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: selfSignedCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
} -->

