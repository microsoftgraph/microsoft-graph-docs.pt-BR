---
title: Obter managedDeviceMobileAppConfigurationDeviceSummary
description: Ler propriedades e relações do objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
ms.openlocfilehash: c435fcb8c91b540fc8fa07b1ee9660bf193b7bc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306031"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="d5fea-103">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d5fea-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="d5fea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5fea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5fea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5fea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5fea-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d5fea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5fea-107">Ler propriedades e relações do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d5fea-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5fea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5fea-108">Prerequisites</span></span>
<span data-ttu-id="d5fea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5fea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5fea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5fea-111">Permission type</span></span>|<span data-ttu-id="d5fea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5fea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5fea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5fea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5fea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5fea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d5fea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5fea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5fea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5fea-116">Not supported.</span></span>|
|<span data-ttu-id="d5fea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5fea-117">Application</span></span>|<span data-ttu-id="d5fea-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5fea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5fea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5fea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5fea-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5fea-120">Optional query parameters</span></span>
<span data-ttu-id="d5fea-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5fea-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d5fea-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5fea-122">Request headers</span></span>
|<span data-ttu-id="d5fea-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5fea-123">Header</span></span>|<span data-ttu-id="d5fea-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d5fea-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5fea-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5fea-125">Authorization</span></span>|<span data-ttu-id="d5fea-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5fea-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5fea-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d5fea-127">Accept</span></span>|<span data-ttu-id="d5fea-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d5fea-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5fea-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5fea-129">Request body</span></span>
<span data-ttu-id="d5fea-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5fea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5fea-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5fea-131">Response</span></span>
<span data-ttu-id="d5fea-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5fea-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5fea-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5fea-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5fea-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5fea-134">Request</span></span>
<span data-ttu-id="d5fea-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5fea-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="d5fea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5fea-136">Response</span></span>
<span data-ttu-id="d5fea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5fea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





