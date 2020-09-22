---
title: Função getManagedAppPolicies
description: Obtém as restrições de aplicativo para um determinado usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32e8ce11f9e644407c588005f55eed53f1c6a435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020843"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="77431-103">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="77431-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="77431-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77431-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77431-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77431-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77431-106">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="77431-106">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77431-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77431-107">Prerequisites</span></span>
<span data-ttu-id="77431-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77431-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77431-110">Permission type</span></span>|<span data-ttu-id="77431-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77431-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77431-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77431-112">Delegated (work or school account)</span></span>| <span data-ttu-id="77431-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="77431-113">_varies by context_</span></span>|
| <span data-ttu-id="77431-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="77431-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="77431-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77431-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="77431-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77431-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77431-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77431-117">Not supported.</span></span>|
|<span data-ttu-id="77431-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77431-118">Application</span></span>|<span data-ttu-id="77431-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77431-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77431-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77431-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="77431-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77431-121">Request headers</span></span>
|<span data-ttu-id="77431-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77431-122">Header</span></span>|<span data-ttu-id="77431-123">Valor</span><span class="sxs-lookup"><span data-stu-id="77431-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77431-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="77431-124">Authorization</span></span>|<span data-ttu-id="77431-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77431-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77431-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77431-126">Accept</span></span>|<span data-ttu-id="77431-127">application/json</span><span class="sxs-lookup"><span data-stu-id="77431-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77431-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77431-128">Request body</span></span>
<span data-ttu-id="77431-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77431-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77431-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="77431-130">Response</span></span>
<span data-ttu-id="77431-131">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77431-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77431-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77431-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="77431-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77431-133">Request</span></span>
<span data-ttu-id="77431-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77431-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="77431-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="77431-135">Response</span></span>
<span data-ttu-id="77431-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77431-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```









