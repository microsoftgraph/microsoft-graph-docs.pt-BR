---
title: Listar managedDeviceMobileAppConfigurationAssignments
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 577f2afeb482f848b529688c97798342d9eafb25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445152"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="f8e89-103">Listar managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="f8e89-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="f8e89-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8e89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8e89-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8e89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8e89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8e89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e89-107">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8e89-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8e89-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8e89-108">Prerequisites</span></span>
<span data-ttu-id="f8e89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8e89-111">Permission type</span></span>|<span data-ttu-id="f8e89-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8e89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8e89-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8e89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8e89-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e89-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8e89-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8e89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8e89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8e89-116">Not supported.</span></span>|
|<span data-ttu-id="f8e89-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8e89-117">Application</span></span>|<span data-ttu-id="f8e89-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e89-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8e89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8e89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f8e89-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e89-120">Request headers</span></span>
|<span data-ttu-id="f8e89-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8e89-121">Header</span></span>|<span data-ttu-id="f8e89-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8e89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8e89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8e89-123">Authorization</span></span>|<span data-ttu-id="f8e89-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8e89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8e89-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8e89-125">Accept</span></span>|<span data-ttu-id="f8e89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8e89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8e89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e89-127">Request body</span></span>
<span data-ttu-id="f8e89-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8e89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8e89-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8e89-129">Response</span></span>
<span data-ttu-id="f8e89-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8e89-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e89-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8e89-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8e89-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e89-132">Request</span></span>
<span data-ttu-id="f8e89-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8e89-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="f8e89-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8e89-134">Response</span></span>
<span data-ttu-id="f8e89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8e89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





