---
title: Listar managedAppPolicies
description: Listar propriedades e relações dos objetos managedAppPolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fece1239c493f9c81c7bd36393648c65c8e134f5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513151"
---
# <a name="list-managedapppolicies"></a><span data-ttu-id="02a53-103">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="02a53-103">List managedAppPolicies</span></span>

<span data-ttu-id="02a53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02a53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02a53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02a53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02a53-106">Listar propriedades e relações dos objetos [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="02a53-106">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02a53-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02a53-107">Prerequisites</span></span>
<span data-ttu-id="02a53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a53-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02a53-110">Permission type</span></span>|<span data-ttu-id="02a53-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02a53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a53-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02a53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02a53-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02a53-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="02a53-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02a53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02a53-115">Not supported.</span></span>|
|<span data-ttu-id="02a53-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02a53-116">Application</span></span>|<span data-ttu-id="02a53-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02a53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a53-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02a53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="02a53-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02a53-119">Request headers</span></span>
|<span data-ttu-id="02a53-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02a53-120">Header</span></span>|<span data-ttu-id="02a53-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02a53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a53-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02a53-122">Authorization</span></span>|<span data-ttu-id="02a53-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02a53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02a53-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02a53-124">Accept</span></span>|<span data-ttu-id="02a53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02a53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02a53-126">Request body</span></span>
<span data-ttu-id="02a53-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02a53-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02a53-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a53-128">Response</span></span>
<span data-ttu-id="02a53-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02a53-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a53-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02a53-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02a53-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02a53-131">Request</span></span>
<span data-ttu-id="02a53-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02a53-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="02a53-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a53-133">Response</span></span>
<span data-ttu-id="02a53-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02a53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




