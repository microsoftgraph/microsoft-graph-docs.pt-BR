---
title: Obter depOnboardingSetting
description: Leia propriedades e relações do objeto depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5264467e3c1794622cf37c7c1c60e0eed86b035
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126231"
---
# <a name="get-deponboardingsetting"></a><span data-ttu-id="0aa95-103">Obter depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="0aa95-103">Get depOnboardingSetting</span></span>

<span data-ttu-id="0aa95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aa95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0aa95-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0aa95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aa95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0aa95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aa95-107">Leia propriedades e relações do objeto [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)</span><span class="sxs-lookup"><span data-stu-id="0aa95-107">Read properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aa95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0aa95-108">Prerequisites</span></span>
<span data-ttu-id="0aa95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aa95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0aa95-111">Permission type</span></span>|<span data-ttu-id="0aa95-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0aa95-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aa95-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0aa95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0aa95-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aa95-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0aa95-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0aa95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aa95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aa95-116">Not supported.</span></span>|
|<span data-ttu-id="0aa95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0aa95-117">Application</span></span>|<span data-ttu-id="0aa95-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aa95-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aa95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0aa95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0aa95-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0aa95-120">Optional query parameters</span></span>
<span data-ttu-id="0aa95-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0aa95-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0aa95-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa95-122">Request headers</span></span>
|<span data-ttu-id="0aa95-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0aa95-123">Header</span></span>|<span data-ttu-id="0aa95-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0aa95-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aa95-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0aa95-125">Authorization</span></span>|<span data-ttu-id="0aa95-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0aa95-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aa95-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0aa95-127">Accept</span></span>|<span data-ttu-id="0aa95-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0aa95-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aa95-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa95-129">Request body</span></span>
<span data-ttu-id="0aa95-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0aa95-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aa95-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa95-131">Response</span></span>
<span data-ttu-id="0aa95-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um objeto depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aa95-132">If successful, this method returns a `200 OK` response code and [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aa95-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0aa95-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aa95-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa95-134">Request</span></span>
<span data-ttu-id="0aa95-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aa95-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

### <a name="response"></a><span data-ttu-id="0aa95-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa95-136">Response</span></span>
<span data-ttu-id="0aa95-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0aa95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




