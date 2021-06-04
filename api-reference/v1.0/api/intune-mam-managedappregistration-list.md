---
title: Listar managedAppRegistrations
description: Listar propriedades e relações dos objetos managedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39bb2b892ca6ade49917b5c13c11677c985bfbbc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752816"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="e76a3-103">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="e76a3-103">List managedAppRegistrations</span></span>

<span data-ttu-id="e76a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e76a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e76a3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e76a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76a3-106">Listar propriedades e relações dos objetos [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e76a3-106">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e76a3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e76a3-107">Prerequisites</span></span>
<span data-ttu-id="e76a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e76a3-110">Permission type</span></span>|<span data-ttu-id="e76a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e76a3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e76a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e76a3-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76a3-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e76a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e76a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e76a3-115">Not supported.</span></span>|
|<span data-ttu-id="e76a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e76a3-116">Application</span></span>|<span data-ttu-id="e76a3-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76a3-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e76a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="e76a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e76a3-119">Request headers</span></span>
|<span data-ttu-id="e76a3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e76a3-120">Header</span></span>|<span data-ttu-id="e76a3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e76a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76a3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e76a3-122">Authorization</span></span>|<span data-ttu-id="e76a3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e76a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76a3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e76a3-124">Accept</span></span>|<span data-ttu-id="e76a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e76a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76a3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e76a3-126">Request body</span></span>
<span data-ttu-id="e76a3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e76a3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e76a3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e76a3-128">Response</span></span>
<span data-ttu-id="e76a3-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppRegistration](../resources/intune-mam-managedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e76a3-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76a3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e76a3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e76a3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e76a3-131">Request</span></span>
<span data-ttu-id="e76a3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e76a3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="e76a3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e76a3-133">Response</span></span>
<span data-ttu-id="e76a3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e76a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```




