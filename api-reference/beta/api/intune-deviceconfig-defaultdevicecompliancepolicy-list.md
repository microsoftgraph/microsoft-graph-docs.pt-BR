---
title: Lista defaultDeviceCompliancePolicies
description: Lista as propriedades e os relacionamentos dos objetos defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 00dd404b9f768efda9b7a153bb11f39057571493
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813787"
---
# <a name="list-defaultdevicecompliancepolicies"></a><span data-ttu-id="ef333-103">Lista defaultDeviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="ef333-103">List defaultDeviceCompliancePolicies</span></span>

> <span data-ttu-id="ef333-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef333-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef333-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef333-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef333-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef333-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef333-107">Lista as propriedades e os relacionamentos dos objetos [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ef333-107">List properties and relationships of the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef333-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef333-108">Prerequisites</span></span>
<span data-ttu-id="ef333-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef333-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef333-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef333-111">Permission type</span></span>|<span data-ttu-id="ef333-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef333-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef333-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef333-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef333-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef333-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef333-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef333-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef333-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef333-116">Not supported.</span></span>|
|<span data-ttu-id="ef333-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef333-117">Application</span></span>|<span data-ttu-id="ef333-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef333-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef333-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef333-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ef333-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef333-120">Request headers</span></span>
|<span data-ttu-id="ef333-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef333-121">Header</span></span>|<span data-ttu-id="ef333-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef333-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef333-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef333-123">Authorization</span></span>|<span data-ttu-id="ef333-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef333-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef333-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef333-125">Accept</span></span>|<span data-ttu-id="ef333-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef333-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef333-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef333-127">Request body</span></span>
<span data-ttu-id="ef333-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef333-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef333-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef333-129">Response</span></span>
<span data-ttu-id="ef333-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef333-130">If successful, this method returns a `200 OK` response code and a collection of [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef333-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef333-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef333-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef333-132">Request</span></span>
<span data-ttu-id="ef333-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef333-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="ef333-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef333-134">Response</span></span>
<span data-ttu-id="ef333-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef333-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "a285f027-f027-a285-27f0-85a227f085a2",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```





