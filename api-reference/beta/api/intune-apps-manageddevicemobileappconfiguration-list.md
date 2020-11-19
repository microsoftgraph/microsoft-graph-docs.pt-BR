---
title: Listar managedDeviceMobileAppConfigurations
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2247883d444364c3ac2aa683582137993477b4ba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250461"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="4f775-103">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="4f775-103">List managedDeviceMobileAppConfigurations</span></span>

<span data-ttu-id="4f775-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f775-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f775-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f775-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f775-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f775-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f775-107">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f775-107">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f775-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f775-108">Prerequisites</span></span>
<span data-ttu-id="4f775-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f775-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f775-111">Permission type</span></span>|<span data-ttu-id="4f775-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f775-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f775-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f775-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f775-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f775-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4f775-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f775-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f775-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f775-116">Not supported.</span></span>|
|<span data-ttu-id="4f775-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f775-117">Application</span></span>|<span data-ttu-id="4f775-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f775-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f775-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f775-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f775-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f775-120">Request headers</span></span>
|<span data-ttu-id="4f775-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f775-121">Header</span></span>|<span data-ttu-id="4f775-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f775-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f775-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f775-123">Authorization</span></span>|<span data-ttu-id="4f775-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f775-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f775-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f775-125">Accept</span></span>|<span data-ttu-id="4f775-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f775-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f775-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f775-127">Request body</span></span>
<span data-ttu-id="4f775-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f775-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f775-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f775-129">Response</span></span>
<span data-ttu-id="4f775-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f775-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f775-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f775-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f775-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f775-132">Request</span></span>
<span data-ttu-id="4f775-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f775-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="4f775-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f775-134">Response</span></span>
<span data-ttu-id="4f775-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f775-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
      "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




