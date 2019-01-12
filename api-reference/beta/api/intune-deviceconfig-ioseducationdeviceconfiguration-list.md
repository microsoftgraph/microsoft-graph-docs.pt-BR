---
title: Lista iosEducationDeviceConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosEducationDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 26c2a6ff2c249f5e7261a0b33ee6530870fd81c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953599"
---
# <a name="list-ioseducationdeviceconfigurations"></a><span data-ttu-id="a1fbf-103">Lista iosEducationDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="a1fbf-103">List iosEducationDeviceConfigurations</span></span>

> <span data-ttu-id="a1fbf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1fbf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1fbf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1fbf-107">Lista as propriedades e os relacionamentos dos objetos [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a1fbf-107">List properties and relationships of the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1fbf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1fbf-108">Prerequisites</span></span>
<span data-ttu-id="a1fbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1fbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1fbf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1fbf-111">Permission type</span></span>|<span data-ttu-id="a1fbf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1fbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1fbf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1fbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1fbf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1fbf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1fbf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1fbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1fbf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-116">Not supported.</span></span>|
|<span data-ttu-id="a1fbf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1fbf-117">Application</span></span>|<span data-ttu-id="a1fbf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1fbf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1fbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1fbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1fbf-120">Request headers</span></span>
|<span data-ttu-id="a1fbf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1fbf-121">Header</span></span>|<span data-ttu-id="a1fbf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1fbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1fbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1fbf-123">Authorization</span></span>|<span data-ttu-id="a1fbf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1fbf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1fbf-125">Accept</span></span>|<span data-ttu-id="a1fbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1fbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1fbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1fbf-127">Request body</span></span>
<span data-ttu-id="a1fbf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1fbf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1fbf-129">Response</span></span>
<span data-ttu-id="a1fbf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-130">If successful, this method returns a `200 OK` response code and a collection of [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1fbf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1fbf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1fbf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1fbf-132">Request</span></span>
<span data-ttu-id="a1fbf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a1fbf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1fbf-134">Response</span></span>
<span data-ttu-id="a1fbf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1fbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 510

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
      "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```





