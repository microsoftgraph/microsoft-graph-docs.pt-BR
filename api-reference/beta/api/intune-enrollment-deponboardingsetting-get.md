---
title: Obter depOnboardingSetting
description: Leia as propriedades e as relações do objeto depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 933cd6c2ed0e11f1230f532499cb21483f5c25ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533273"
---
# <a name="get-deponboardingsetting"></a><span data-ttu-id="85072-103">Obter depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="85072-103">Get depOnboardingSetting</span></span>

> <span data-ttu-id="85072-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85072-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85072-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85072-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85072-106">Leia as propriedades e as relações do objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="85072-106">Read properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85072-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85072-107">Prerequisites</span></span>
<span data-ttu-id="85072-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85072-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85072-110">Permission type</span></span>|<span data-ttu-id="85072-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85072-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85072-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85072-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85072-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85072-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="85072-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85072-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85072-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85072-115">Not supported.</span></span>|
|<span data-ttu-id="85072-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85072-116">Application</span></span>|<span data-ttu-id="85072-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85072-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85072-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85072-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85072-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85072-119">Optional query parameters</span></span>
<span data-ttu-id="85072-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85072-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85072-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85072-121">Request headers</span></span>
|<span data-ttu-id="85072-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85072-122">Header</span></span>|<span data-ttu-id="85072-123">Valor</span><span class="sxs-lookup"><span data-stu-id="85072-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85072-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="85072-124">Authorization</span></span>|<span data-ttu-id="85072-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85072-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85072-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85072-126">Accept</span></span>|<span data-ttu-id="85072-127">application/json</span><span class="sxs-lookup"><span data-stu-id="85072-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85072-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85072-128">Request body</span></span>
<span data-ttu-id="85072-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85072-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85072-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="85072-130">Response</span></span>
<span data-ttu-id="85072-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85072-131">If successful, this method returns a `200 OK` response code and [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85072-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85072-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="85072-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85072-133">Request</span></span>
<span data-ttu-id="85072-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85072-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

### <a name="response"></a><span data-ttu-id="85072-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="85072-135">Response</span></span>
<span data-ttu-id="85072-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85072-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 740

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
    "dataSharingConsentGranted": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```





