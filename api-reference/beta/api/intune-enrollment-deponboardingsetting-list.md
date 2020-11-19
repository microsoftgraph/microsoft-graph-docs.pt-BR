---
title: Listar depOnboardingSettings
description: Listar Propriedades e relações dos objetos depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f98b5218b47b1daeaea0cefbc2639acfce6452fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309639"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="f5ba4-103">Listar depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="f5ba4-103">List depOnboardingSettings</span></span>

<span data-ttu-id="f5ba4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ba4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5ba4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5ba4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ba4-107">Listar Propriedades e relações dos objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ba4-107">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5ba4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5ba4-108">Prerequisites</span></span>
<span data-ttu-id="f5ba4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ba4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5ba4-111">Permission type</span></span>|<span data-ttu-id="f5ba4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5ba4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5ba4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5ba4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5ba4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5ba4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f5ba4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5ba4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5ba4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-116">Not supported.</span></span>|
|<span data-ttu-id="f5ba4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5ba4-117">Application</span></span>|<span data-ttu-id="f5ba4-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5ba4-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5ba4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ba4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="f5ba4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ba4-120">Request headers</span></span>
|<span data-ttu-id="f5ba4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5ba4-121">Header</span></span>|<span data-ttu-id="f5ba4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5ba4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5ba4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ba4-123">Authorization</span></span>|<span data-ttu-id="f5ba4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5ba4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5ba4-125">Accept</span></span>|<span data-ttu-id="f5ba4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5ba4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ba4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ba4-127">Request body</span></span>
<span data-ttu-id="f5ba4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5ba4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ba4-129">Response</span></span>
<span data-ttu-id="f5ba4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-130">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5ba4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5ba4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5ba4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ba4-132">Request</span></span>
<span data-ttu-id="f5ba4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="f5ba4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ba4-134">Response</span></span>
<span data-ttu-id="f5ba4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5ba4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
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
  ]
}
```




