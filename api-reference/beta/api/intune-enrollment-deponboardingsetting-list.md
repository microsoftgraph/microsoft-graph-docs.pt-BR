---
title: Lista depOnboardingSettings
description: Lista as propriedades e os relacionamentos dos objetos depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a8602215456a2331f9a05985c56763aea0c2c345
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964127"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="a98ba-103">Lista depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="a98ba-103">List depOnboardingSettings</span></span>

> <span data-ttu-id="a98ba-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a98ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a98ba-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a98ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a98ba-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a98ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a98ba-107">Lista as propriedades e os relacionamentos dos objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="a98ba-107">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a98ba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a98ba-108">Prerequisites</span></span>
<span data-ttu-id="a98ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a98ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a98ba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a98ba-111">Permission type</span></span>|<span data-ttu-id="a98ba-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a98ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a98ba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a98ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a98ba-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98ba-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a98ba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a98ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a98ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a98ba-116">Not supported.</span></span>|
|<span data-ttu-id="a98ba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a98ba-117">Application</span></span>|<span data-ttu-id="a98ba-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a98ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a98ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a98ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="a98ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a98ba-120">Request headers</span></span>
|<span data-ttu-id="a98ba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a98ba-121">Header</span></span>|<span data-ttu-id="a98ba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a98ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a98ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a98ba-123">Authorization</span></span>|<span data-ttu-id="a98ba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a98ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a98ba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a98ba-125">Accept</span></span>|<span data-ttu-id="a98ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a98ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a98ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a98ba-127">Request body</span></span>
<span data-ttu-id="a98ba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a98ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a98ba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a98ba-129">Response</span></span>
<span data-ttu-id="a98ba-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a98ba-130">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a98ba-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a98ba-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a98ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a98ba-132">Request</span></span>
<span data-ttu-id="a98ba-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a98ba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="a98ba-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a98ba-134">Response</span></span>
<span data-ttu-id="a98ba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a98ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "defaultProfileDisplayName": "Default Profile Display Name value",
      "dataSharingConsentGranted": true
    }
  ]
}
```





