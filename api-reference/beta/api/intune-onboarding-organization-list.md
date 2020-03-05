---
title: Listar organizations
description: Listar propriedades e relações de objetos de organização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 375fbc66109df47752c01a9cdf07fb2b57cf51c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461862"
---
# <a name="list-organizations"></a><span data-ttu-id="fc3c1-103">Listar organizations</span><span class="sxs-lookup"><span data-stu-id="fc3c1-103">List organizations</span></span>

<span data-ttu-id="fc3c1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc3c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc3c1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc3c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc3c1-107">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="fc3c1-107">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc3c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc3c1-108">Prerequisites</span></span>
<span data-ttu-id="fc3c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc3c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc3c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc3c1-111">Permission type</span></span>|<span data-ttu-id="fc3c1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc3c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc3c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc3c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc3c1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc3c1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fc3c1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc3c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc3c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-116">Not supported.</span></span>|
|<span data-ttu-id="fc3c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc3c1-117">Application</span></span>|<span data-ttu-id="fc3c1-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc3c1-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc3c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="fc3c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3c1-120">Request headers</span></span>
|<span data-ttu-id="fc3c1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc3c1-121">Header</span></span>|<span data-ttu-id="fc3c1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fc3c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc3c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc3c1-123">Authorization</span></span>|<span data-ttu-id="fc3c1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc3c1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc3c1-125">Accept</span></span>|<span data-ttu-id="fc3c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc3c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc3c1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3c1-127">Request body</span></span>
<span data-ttu-id="fc3c1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc3c1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3c1-129">Response</span></span>
<span data-ttu-id="fc3c1-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-130">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc3c1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc3c1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc3c1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3c1-132">Request</span></span>
<span data-ttu-id="fc3c1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization
```

### <a name="response"></a><span data-ttu-id="fc3c1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3c1-134">Response</span></span>
<span data-ttu-id="fc3c1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc3c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune",
      "certificateConnectorSetting": {
        "@odata.type": "microsoft.graph.certificateConnectorSetting",
        "status": 6,
        "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
        "enrollmentError": "Enrollment Error value",
        "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
        "connectorVersion": "Connector Version value",
        "lastUploadVersion": 1
      }
    }
  ]
}
```





