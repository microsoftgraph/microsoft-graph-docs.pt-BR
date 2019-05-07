---
title: Obter entrada
description: Descreve o método Get do recurso de entrada (entidade) da API do Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d1971a0c0dd85ab07ff7a23204b31c141c130a62
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629723"
---
# <a name="get-signin"></a><span data-ttu-id="c0426-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="c0426-103">Get signIn</span></span>

<span data-ttu-id="c0426-104">Recupere um evento específico de logon de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="c0426-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="c0426-105">As entradas interativas por natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e os logins federados bem-sucedidos estão incluídos atualmente nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="c0426-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0426-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0426-106">Permissions</span></span>

<span data-ttu-id="c0426-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="c0426-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="c0426-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0426-109">Permission type</span></span>      | <span data-ttu-id="c0426-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0426-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0426-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0426-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0426-112">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="c0426-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="c0426-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0426-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0426-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c0426-114">Not supported</span></span>   |
|<span data-ttu-id="c0426-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0426-115">Application</span></span> | <span data-ttu-id="c0426-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0426-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0426-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0426-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0426-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0426-118">Optional query parameters</span></span>

<span data-ttu-id="c0426-119">Este método dá suporte a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0426-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="c0426-120">Para obter detalhes sobre como usar esses parâmetros, confira [parâmetros de consulta OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="c0426-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0426-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0426-121">Request headers</span></span>

| <span data-ttu-id="c0426-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c0426-122">Name</span></span>      |<span data-ttu-id="c0426-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0426-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0426-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0426-124">Authorization</span></span>  | <span data-ttu-id="c0426-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c0426-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0426-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0426-126">Request body</span></span>

<span data-ttu-id="c0426-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0426-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0426-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0426-128">Response</span></span>

<span data-ttu-id="c0426-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0426-129">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0426-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0426-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0426-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0426-131">Request</span></span>

<span data-ttu-id="c0426-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0426-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="c0426-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0426-133">Response</span></span>

<span data-ttu-id="c0426-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0426-134">Here is an example of the response.</span></span>
><span data-ttu-id="c0426-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0426-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
```

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "id": "id",
    "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
    "appDisplayName": "Azure",
    "createdDateTime": "2018-01-09T21:17:21.5077253Z",
    "clientAppUsed": null,
    "conditionalAccessApplied": true,
    "conditionalAccessPolicies": [{
        "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
        "displayName": "capPolicy",
        "enforcedAccessControls": ["MFA", "TOU"],
        "enforcedSessionControls": ["CloudAppSecurity"],
        "result": "success"
    }],
    "correlationId": "17444d3c-563d-4b08-ac20-815892b87e42",
    "deviceDetail": {
        "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
        "displayName": "DeviceName",
        "operatingSystem": "Windows 10",
        "browser": "Rich Client v3.14.1592.7",
        "isCompliant": true,
        "isManaged": true,
        "trustType": ""
    },
    "ipAddress": "127.0.0.1",
    "location": {
        "city": "Redmond",
        "state": "WA",
        "countryOrRegion": "USA",
        "geoCoordinates": {
            "altitude": 41.589,
            "latitude": 41.589,
            "longitude": -93.6151
        }
    },
    "status": {
        "errorCode": 0,
        "failureReason": null,
        "additionalDetails": "SignIn Success & CA Success"
    },
    "userDisplayName": "Jamie Doe",
    "userPrincipalName": "jdoe@wingtiptoys.com",
    "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
