---
title: Listar organizations
description: Listar propriedades e relações de objetos de organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 22ba561f66f6c1657cefa684ffb2e365738eaab7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695450"
---
# <a name="list-organizations"></a><span data-ttu-id="fdc70-103">Listar organizations</span><span class="sxs-lookup"><span data-stu-id="fdc70-103">List organizations</span></span>

<span data-ttu-id="fdc70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdc70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdc70-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fdc70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdc70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdc70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc70-107">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="fdc70-107">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdc70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdc70-108">Prerequisites</span></span>
<span data-ttu-id="fdc70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdc70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdc70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdc70-111">Permission type</span></span>|<span data-ttu-id="fdc70-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdc70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdc70-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdc70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdc70-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdc70-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fdc70-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdc70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdc70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdc70-116">Not supported.</span></span>|
|<span data-ttu-id="fdc70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdc70-117">Application</span></span>|<span data-ttu-id="fdc70-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdc70-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdc70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdc70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="fdc70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdc70-120">Request headers</span></span>
|<span data-ttu-id="fdc70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdc70-121">Header</span></span>|<span data-ttu-id="fdc70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdc70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdc70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdc70-123">Authorization</span></span>|<span data-ttu-id="fdc70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdc70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdc70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdc70-125">Accept</span></span>|<span data-ttu-id="fdc70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdc70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdc70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdc70-127">Request body</span></span>
<span data-ttu-id="fdc70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdc70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdc70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdc70-129">Response</span></span>
<span data-ttu-id="fdc70-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdc70-130">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdc70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdc70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdc70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdc70-132">Request</span></span>
<span data-ttu-id="fdc70-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdc70-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization
```

### <a name="response"></a><span data-ttu-id="fdc70-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdc70-134">Response</span></span>
<span data-ttu-id="fdc70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdc70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





