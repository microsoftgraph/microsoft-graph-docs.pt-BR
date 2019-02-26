---
title: Função getManagedAppPolicies
description: Obtém as restrições de aplicativo para um determinado usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94448fa6f89935e0577b91f9f49dc319b959b09e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260015"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="f4c94-103">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="f4c94-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="f4c94-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4c94-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4c94-105">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="f4c94-105">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4c94-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4c94-106">Prerequisites</span></span>
<span data-ttu-id="f4c94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4c94-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4c94-109">Permission type</span></span>|<span data-ttu-id="f4c94-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4c94-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4c94-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4c94-111">Delegated (work or school account)</span></span>| <span data-ttu-id="f4c94-112">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="f4c94-112">_varies by context_</span></span>|
| <span data-ttu-id="f4c94-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="f4c94-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="f4c94-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c94-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="f4c94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4c94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4c94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4c94-116">Not supported.</span></span>|
|<span data-ttu-id="f4c94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4c94-117">Application</span></span>|<span data-ttu-id="f4c94-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4c94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4c94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f4c94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c94-120">Request headers</span></span>
|<span data-ttu-id="f4c94-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4c94-121">Header</span></span>|<span data-ttu-id="f4c94-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4c94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4c94-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4c94-123">Authorization</span></span>|<span data-ttu-id="f4c94-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4c94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4c94-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4c94-125">Accept</span></span>|<span data-ttu-id="f4c94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4c94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4c94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c94-127">Request body</span></span>
<span data-ttu-id="f4c94-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4c94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c94-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4c94-129">Response</span></span>
<span data-ttu-id="f4c94-130">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4c94-130">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4c94-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4c94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4c94-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c94-132">Request</span></span>
<span data-ttu-id="f4c94-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4c94-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="f4c94-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4c94-134">Response</span></span>
<span data-ttu-id="f4c94-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4c94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



