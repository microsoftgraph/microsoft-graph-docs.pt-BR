---
title: Listar iosUpdateConfigurations
description: Listar propriedades e relações dos objetos iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4aa7f147583ae128c70e4fb221dd3bc0e3731665
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869108"
---
# <a name="list-iosupdateconfigurations"></a><span data-ttu-id="43e30-103">Listar iosUpdateConfigurations</span><span class="sxs-lookup"><span data-stu-id="43e30-103">List iosUpdateConfigurations</span></span>

> <span data-ttu-id="43e30-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43e30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43e30-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43e30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43e30-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43e30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43e30-107">Listar propriedades e relações dos objetos [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43e30-107">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43e30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43e30-108">Prerequisites</span></span>
<span data-ttu-id="43e30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43e30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43e30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43e30-111">Permission type</span></span>|<span data-ttu-id="43e30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43e30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43e30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43e30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43e30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43e30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43e30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43e30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43e30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43e30-116">Not supported.</span></span>|
|<span data-ttu-id="43e30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43e30-117">Application</span></span>|<span data-ttu-id="43e30-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43e30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43e30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43e30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43e30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43e30-120">Request headers</span></span>
|<span data-ttu-id="43e30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43e30-121">Header</span></span>|<span data-ttu-id="43e30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="43e30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43e30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43e30-123">Authorization</span></span>|<span data-ttu-id="43e30-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43e30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43e30-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43e30-125">Accept</span></span>|<span data-ttu-id="43e30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43e30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43e30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43e30-127">Request body</span></span>
<span data-ttu-id="43e30-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43e30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43e30-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="43e30-129">Response</span></span>
<span data-ttu-id="43e30-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43e30-130">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43e30-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43e30-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="43e30-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43e30-132">Request</span></span>
<span data-ttu-id="43e30-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43e30-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="43e30-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="43e30-134">Response</span></span>
<span data-ttu-id="43e30-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43e30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
      "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "isEnabled": true,
      "activeHoursStart": "12:00:05.5020000",
      "activeHoursEnd": "11:59:00.8990000",
      "scheduledInstallDays": [
        "monday"
      ],
      "utcTimeOffsetInMinutes": 6,
      "enforcedSoftwareUpdateDelayInDays": 1
    }
  ]
}
```





