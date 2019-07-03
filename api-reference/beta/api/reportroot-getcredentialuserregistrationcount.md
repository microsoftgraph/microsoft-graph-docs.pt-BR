---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: b5e14b293447e585451f343a1c130e7d3d323a59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499265"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="40b73-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="40b73-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b73-104">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="40b73-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="40b73-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="40b73-105">Permissions</span></span>

<span data-ttu-id="40b73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40b73-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40b73-108">Permission type</span></span>                        | <span data-ttu-id="40b73-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40b73-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="40b73-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40b73-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="40b73-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40b73-111">Reports.Read.All</span></span> |
| <span data-ttu-id="40b73-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40b73-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40b73-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40b73-113">Not supported.</span></span> |
| <span data-ttu-id="40b73-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40b73-114">Application</span></span>                            | <span data-ttu-id="40b73-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40b73-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40b73-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40b73-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialsUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="40b73-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40b73-117">Request headers</span></span>

| <span data-ttu-id="40b73-118">Nome</span><span class="sxs-lookup"><span data-stu-id="40b73-118">Name</span></span>          | <span data-ttu-id="40b73-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b73-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="40b73-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="40b73-120">Authorization</span></span> | <span data-ttu-id="40b73-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="40b73-121">Bearer {token}</span></span> |
| <span data-ttu-id="40b73-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40b73-122">Content-Type</span></span> | <span data-ttu-id="40b73-123">application/json</span><span class="sxs-lookup"><span data-stu-id="40b73-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="40b73-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40b73-124">Request body</span></span>

<span data-ttu-id="40b73-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40b73-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40b73-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="40b73-126">Response</span></span>

<span data-ttu-id="40b73-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40b73-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40b73-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="40b73-128">Examples</span></span>

<span data-ttu-id="40b73-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="40b73-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="40b73-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40b73-130">Request</span></span>

<span data-ttu-id="40b73-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="40b73-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```

### <a name="response"></a><span data-ttu-id="40b73-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="40b73-132">Response</span></span>

<span data-ttu-id="40b73-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="40b73-133">The following is an example of the response.</span></span>

> <span data-ttu-id="40b73-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40b73-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40b73-135">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40b73-135">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationCount)",
  "value": [
    {
      "id" : "id-value",
      "totalUserCount" : 23123,
      "userRegistrationCounts" :
      [
        { "userRegistrationStatus":"registered", 
          "userRegistationCount": 23423 }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUserRegistrationCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
