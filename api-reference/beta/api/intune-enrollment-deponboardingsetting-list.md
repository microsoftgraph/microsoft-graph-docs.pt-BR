---
title: Listar depOnboardingSettings
description: Listar Propriedades e relações dos objetos depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2af4f462b47e5e2993f2a688be8cdd8440facf98
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789630"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="737f0-103">Listar depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="737f0-103">List depOnboardingSettings</span></span>

> <span data-ttu-id="737f0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="737f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="737f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="737f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="737f0-106">Listar Propriedades e relações dos objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="737f0-106">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="737f0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="737f0-107">Prerequisites</span></span>
<span data-ttu-id="737f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="737f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="737f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="737f0-110">Permission type</span></span>|<span data-ttu-id="737f0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="737f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="737f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="737f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="737f0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="737f0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="737f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="737f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="737f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737f0-115">Not supported.</span></span>|
|<span data-ttu-id="737f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="737f0-116">Application</span></span>|<span data-ttu-id="737f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="737f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="737f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="737f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="737f0-119">Request headers</span></span>
|<span data-ttu-id="737f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="737f0-120">Header</span></span>|<span data-ttu-id="737f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="737f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="737f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="737f0-122">Authorization</span></span>|<span data-ttu-id="737f0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="737f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="737f0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="737f0-124">Accept</span></span>|<span data-ttu-id="737f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="737f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="737f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="737f0-126">Request body</span></span>
<span data-ttu-id="737f0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="737f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="737f0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="737f0-128">Response</span></span>
<span data-ttu-id="737f0-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="737f0-129">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="737f0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="737f0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="737f0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="737f0-131">Request</span></span>
<span data-ttu-id="737f0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="737f0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="737f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="737f0-133">Response</span></span>
<span data-ttu-id="737f0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="737f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





