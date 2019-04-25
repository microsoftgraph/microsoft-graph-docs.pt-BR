---
title: Listar organizations
description: Listar propriedades e relações de objetos de organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 067489dad7e08053cd4e6004f1e8b20fca479853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528502"
---
# <a name="list-organizations"></a><span data-ttu-id="3b3a2-103">Listar organizations</span><span class="sxs-lookup"><span data-stu-id="3b3a2-103">List organizations</span></span>

> <span data-ttu-id="3b3a2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b3a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b3a2-106">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="3b3a2-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b3a2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b3a2-107">Prerequisites</span></span>
<span data-ttu-id="3b3a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b3a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b3a2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b3a2-110">Permission type</span></span>|<span data-ttu-id="3b3a2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b3a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b3a2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b3a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b3a2-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b3a2-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3b3a2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b3a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b3a2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-115">Not supported.</span></span>|
|<span data-ttu-id="3b3a2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b3a2-116">Application</span></span>|<span data-ttu-id="3b3a2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b3a2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b3a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="3b3a2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3a2-119">Request headers</span></span>
|<span data-ttu-id="3b3a2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b3a2-120">Header</span></span>|<span data-ttu-id="3b3a2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b3a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b3a2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b3a2-122">Authorization</span></span>|<span data-ttu-id="3b3a2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b3a2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b3a2-124">Accept</span></span>|<span data-ttu-id="3b3a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b3a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b3a2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3a2-126">Request body</span></span>
<span data-ttu-id="3b3a2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b3a2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3a2-128">Response</span></span>
<span data-ttu-id="3b3a2-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b3a2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b3a2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b3a2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3a2-131">Request</span></span>
<span data-ttu-id="3b3a2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization
```

### <a name="response"></a><span data-ttu-id="3b3a2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3a2-133">Response</span></span>
<span data-ttu-id="3b3a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b3a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





