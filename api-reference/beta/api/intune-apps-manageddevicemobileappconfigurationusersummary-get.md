---
title: Acessar managedDeviceMobileAppConfigurationUserSummary
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eaf579920de6188c7a60b1f71975adea090c5ed3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984861"
---
# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="75ee7-103">Acessar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="75ee7-103">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="75ee7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75ee7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75ee7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75ee7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75ee7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="75ee7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75ee7-107">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="75ee7-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75ee7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75ee7-108">Prerequisites</span></span>
<span data-ttu-id="75ee7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ee7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ee7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75ee7-111">Permission type</span></span>|<span data-ttu-id="75ee7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75ee7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75ee7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75ee7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75ee7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="75ee7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="75ee7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75ee7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75ee7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75ee7-116">Not supported.</span></span>|
|<span data-ttu-id="75ee7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75ee7-117">Application</span></span>|<span data-ttu-id="75ee7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75ee7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75ee7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75ee7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75ee7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="75ee7-120">Optional query parameters</span></span>
<span data-ttu-id="75ee7-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="75ee7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="75ee7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75ee7-122">Request headers</span></span>
|<span data-ttu-id="75ee7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75ee7-123">Header</span></span>|<span data-ttu-id="75ee7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="75ee7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75ee7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="75ee7-125">Authorization</span></span>|<span data-ttu-id="75ee7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75ee7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75ee7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75ee7-127">Accept</span></span>|<span data-ttu-id="75ee7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="75ee7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75ee7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75ee7-129">Request body</span></span>
<span data-ttu-id="75ee7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75ee7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75ee7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="75ee7-131">Response</span></span>
<span data-ttu-id="75ee7-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75ee7-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75ee7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75ee7-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="75ee7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75ee7-134">Request</span></span>
<span data-ttu-id="75ee7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75ee7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="75ee7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="75ee7-136">Response</span></span>
<span data-ttu-id="75ee7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75ee7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
    "id": "7b953742-3742-7b95-4237-957b4237957b",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





