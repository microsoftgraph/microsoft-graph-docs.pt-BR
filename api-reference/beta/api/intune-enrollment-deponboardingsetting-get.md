---
title: Obter depOnboardingSetting
description: Leia as propriedades e os relacionamentos do objeto depOnboardingSetting.
author: tfitzmac
ms.openlocfilehash: e56461e8e60c2e7ac5999f56b8beaf592db54645
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340961"
---
# <a name="get-deponboardingsetting"></a><span data-ttu-id="d8bab-103">Obter depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="d8bab-103">Get depOnboardingSetting</span></span>

> <span data-ttu-id="d8bab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8bab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8bab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8bab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8bab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d8bab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8bab-107">Leia as propriedades e os relacionamentos do objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bab-107">Read properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8bab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8bab-108">Prerequisites</span></span>
<span data-ttu-id="d8bab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8bab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8bab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8bab-111">Permission type</span></span>|<span data-ttu-id="d8bab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8bab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8bab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8bab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8bab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8bab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d8bab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8bab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8bab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8bab-116">Not supported.</span></span>|
|<span data-ttu-id="d8bab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8bab-117">Application</span></span>|<span data-ttu-id="d8bab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8bab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8bab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8bab-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d8bab-120">Optional query parameters</span></span>
<span data-ttu-id="d8bab-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d8bab-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8bab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bab-122">Request headers</span></span>
|<span data-ttu-id="d8bab-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8bab-123">Header</span></span>|<span data-ttu-id="d8bab-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d8bab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8bab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8bab-125">Authorization</span></span>|<span data-ttu-id="d8bab-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8bab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8bab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d8bab-127">Accept</span></span>|<span data-ttu-id="d8bab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d8bab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8bab-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bab-129">Request body</span></span>
<span data-ttu-id="d8bab-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8bab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8bab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bab-131">Response</span></span>
<span data-ttu-id="d8bab-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8bab-132">If successful, this method returns a `200 OK` response code and [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8bab-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8bab-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8bab-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bab-134">Request</span></span>
<span data-ttu-id="d8bab-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8bab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

### <a name="response"></a><span data-ttu-id="d8bab-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bab-136">Response</span></span>
<span data-ttu-id="d8bab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8bab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 744

{
  "value": {
    "@odata.type": "#microsoft.graph.depOnboardingSetting",
    "id": "40342229-2229-4034-2922-344029223440",
    "appleIdentifier": "Apple Identifier value",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
    "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
    "shareTokenWithSchoolDataSyncService": true,
    "lastSyncErrorCode": 1,
    "tokenType": "dep",
    "tokenName": "Token Name value",
    "syncedDeviceCount": 1,
    "defaultProfileDisplayName": "Default Profile Display Name value",
    "dataSharingConsentGranted": true
  }
}
```





