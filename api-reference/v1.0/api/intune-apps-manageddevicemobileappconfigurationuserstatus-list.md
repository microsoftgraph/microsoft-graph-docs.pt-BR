---
title: Listar managedDeviceMobileAppConfigurationUserStatuses
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31471db6eea629d09d1a458bafa9e9798a2df2a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578180"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="02afd-103">Listar managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="02afd-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="02afd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02afd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02afd-105">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="02afd-105">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02afd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02afd-106">Prerequisites</span></span>
<span data-ttu-id="02afd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02afd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02afd-109">Permission type</span></span>|<span data-ttu-id="02afd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02afd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02afd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02afd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02afd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02afd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="02afd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02afd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02afd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02afd-114">Not supported.</span></span>|
|<span data-ttu-id="02afd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02afd-115">Application</span></span>|<span data-ttu-id="02afd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02afd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02afd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02afd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="02afd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02afd-118">Request headers</span></span>
|<span data-ttu-id="02afd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02afd-119">Header</span></span>|<span data-ttu-id="02afd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="02afd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02afd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02afd-121">Authorization</span></span>|<span data-ttu-id="02afd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02afd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02afd-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02afd-123">Accept</span></span>|<span data-ttu-id="02afd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="02afd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02afd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02afd-125">Request body</span></span>
<span data-ttu-id="02afd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02afd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02afd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="02afd-127">Response</span></span>
<span data-ttu-id="02afd-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02afd-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02afd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02afd-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="02afd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02afd-130">Request</span></span>
<span data-ttu-id="02afd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02afd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="02afd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="02afd-132">Response</span></span>
<span data-ttu-id="02afd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02afd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



