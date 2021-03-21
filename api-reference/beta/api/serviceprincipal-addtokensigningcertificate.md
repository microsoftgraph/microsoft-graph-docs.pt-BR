---
title: 'servicePrincipal: addTokenSigningCertificate'
description: Adicione um certificado de assinatura a um servicePrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13a8b8f1040bf79205a84b97e7f63a2767253200
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965034"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a><span data-ttu-id="f4eb7-103">servicePrincipal: addTokenSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="f4eb7-103">servicePrincipal: addTokenSigningCertificate</span></span>

<span data-ttu-id="f4eb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4eb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4eb7-105">Cria um certificado de assinatura auto-assinado e retorna um [selfSignedCertificate](../resources/selfsignedcertificate.md), que é a parte pública do certificado gerado.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-105">Creates a self-signed signing certificate and returns a [selfSignedCertificate](../resources/selfsignedcertificate.md), which is the public part of the generated certificate.</span></span> <span data-ttu-id="f4eb7-106">O certificado de assinatura auto-assinado é composto por esses recursos: a chave privada ([keyCredential](../resources/keycredential.md) com uso = 'Sign'), a chave pública ([keyCredential](../resources/keycredential.md) com uso = 'verify') e [a passwordCredential](../resources/passwordcredential.md).</span><span class="sxs-lookup"><span data-stu-id="f4eb7-106">The self-signed signing certificate is composed of these resources: the private key ([keyCredential](../resources/keycredential.md) with usage = 'Sign'), the public key ([keyCredential](../resources/keycredential.md) with usage = 'verify'), and the [passwordCredential](../resources/passwordcredential.md).</span></span> <span data-ttu-id="f4eb7-107">Todos os recursos criados têm o **mesmo customKeyIdentifier**.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-107">All the created resources have the same **customKeyIdentifier**.</span></span>

<span data-ttu-id="f4eb7-108">A **senhaCredential** é usada para abrir a chave pfx/privada.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-108">The **passwordCredential** is used to open the pfx/private key.</span></span> <span data-ttu-id="f4eb7-109">Além disso, ele está associado ao privateKey ter a mesma **keyId**.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-109">Also, it's associated with the privateKey having the same **keyId**.</span></span> <span data-ttu-id="f4eb7-110">O assunto do certificado é um valor constante.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-110">The subject of the certificate is a constant value.</span></span> <span data-ttu-id="f4eb7-111">Ele não será afetado pelo **displayName opcional** fornecido na chamada POST.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-111">It won't be affected by the optional **displayName** provided in the POST call.</span></span> <span data-ttu-id="f4eb7-112">O **startDateTime** é definido para o mesmo horário em que o certificado é criado usando a ação.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-112">The **startDateTime** is set to the same time the certificate is created using the action.</span></span> <span data-ttu-id="f4eb7-113">O **endDateTime** pode ter até três anos após a criação do certificado.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-113">The **endDateTime** can be up to three years after the certificate is created.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4eb7-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4eb7-114">Permissions</span></span>

|<span data-ttu-id="f4eb7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4eb7-115">Permission type</span></span>      | <span data-ttu-id="f4eb7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4eb7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4eb7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4eb7-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f4eb7-118">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4eb7-118">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f4eb7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4eb7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4eb7-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-120">None.</span></span>    |
|<span data-ttu-id="f4eb7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4eb7-121">Application</span></span> | <span data-ttu-id="f4eb7-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4eb7-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f4eb7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4eb7-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a><span data-ttu-id="f4eb7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4eb7-124">Request body</span></span>

<span data-ttu-id="f4eb7-125">No corpo da solicitação, forneça as seguintes propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-125">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="f4eb7-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4eb7-126">Property</span></span>     | <span data-ttu-id="f4eb7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4eb7-127">Type</span></span>   |<span data-ttu-id="f4eb7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4eb7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4eb7-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f4eb7-129">displayName</span></span> | <span data-ttu-id="f4eb7-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4eb7-130">string</span></span> | <span data-ttu-id="f4eb7-131">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-131">Friendly name for the key.</span></span>  <span data-ttu-id="f4eb7-132">Ele deve começar com `CN=` .</span><span class="sxs-lookup"><span data-stu-id="f4eb7-132">It must start with `CN=`.</span></span>|
| <span data-ttu-id="f4eb7-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f4eb7-133">endDateTime</span></span> | <span data-ttu-id="f4eb7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4eb7-134">DateTimeOffset</span></span> |<span data-ttu-id="f4eb7-135">A data e a hora em que a credencial expira.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-135">The date and time when the credential expires.</span></span> <span data-ttu-id="f4eb7-136">Pode ser até 3 anos a partir da data em que o certificado é criado.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-136">It can be up to 3 years from the date the certificate is created.</span></span> <span data-ttu-id="f4eb7-137">Se não for fornecido, o padrão será de três anos a partir do momento da criação.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-137">If not supplied, the default is three years from the time of creation.</span></span> <span data-ttu-id="f4eb7-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4eb7-139">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z' .</span><span class="sxs-lookup"><span data-stu-id="f4eb7-139">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z' .</span></span>|

## <a name="response"></a><span data-ttu-id="f4eb7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4eb7-140">Response</span></span>

<span data-ttu-id="f4eb7-141">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [selfSignedCertificate](../resources/selfsignedcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-141">If successful, this method returns a `200 OK` response code and a new [selfSignedCertificate](../resources/selfsignedcertificate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4eb7-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f4eb7-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4eb7-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4eb7-143">Request</span></span>

<span data-ttu-id="f4eb7-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/7c8d4399-b4bf-413a-8b6a-c577790cae7d/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```


### <a name="response"></a><span data-ttu-id="f4eb7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4eb7-145">Response</span></span>

<span data-ttu-id="f4eb7-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f4eb7-146">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.selfSignedCertificate"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "customKeyIdentifier": null,
    "displayName": "customDisplayName",
    "endDateTime": "2023-06-29T00:00:00Z",
    "key": null,
    "keyId": "b859fc29-969f-48b2-9a27-8399b69f441e",
    "startDateTime": "2020-06-29T00:00:00Z",
    "type": "AsymmetricX509Cert",
    "thumbprint":"QWESRTGFWQWEDSASDTGGSADASDWQW",
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
  "suppressions": [
    "Error: serviceprincipal_selfsignedcertificate:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
} -->

