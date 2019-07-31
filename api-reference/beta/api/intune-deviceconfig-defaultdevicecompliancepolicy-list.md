---
title: Listar defaultDeviceCompliancePolicies
description: Listar Propriedades e relações dos objetos defaultDeviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f74f798a5f58f96185310d1b65c7210d2fa0a3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950095"
---
# <a name="list-defaultdevicecompliancepolicies"></a><span data-ttu-id="0aa31-103">Listar defaultDeviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="0aa31-103">List defaultDeviceCompliancePolicies</span></span>

> <span data-ttu-id="0aa31-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0aa31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aa31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0aa31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aa31-106">Listar Propriedades e relações dos objetos [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa31-106">List properties and relationships of the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aa31-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0aa31-107">Prerequisites</span></span>
<span data-ttu-id="0aa31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aa31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0aa31-110">Permission type</span></span>|<span data-ttu-id="0aa31-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0aa31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aa31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0aa31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0aa31-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aa31-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0aa31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0aa31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aa31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aa31-115">Not supported.</span></span>|
|<span data-ttu-id="0aa31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0aa31-116">Application</span></span>|<span data-ttu-id="0aa31-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aa31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aa31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0aa31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0aa31-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa31-119">Request headers</span></span>
|<span data-ttu-id="0aa31-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0aa31-120">Header</span></span>|<span data-ttu-id="0aa31-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0aa31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aa31-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0aa31-122">Authorization</span></span>|<span data-ttu-id="0aa31-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0aa31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aa31-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0aa31-124">Accept</span></span>|<span data-ttu-id="0aa31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0aa31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aa31-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa31-126">Request body</span></span>
<span data-ttu-id="0aa31-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0aa31-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aa31-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa31-128">Response</span></span>
<span data-ttu-id="0aa31-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aa31-129">If successful, this method returns a `200 OK` response code and a collection of [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aa31-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0aa31-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aa31-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa31-131">Request</span></span>
<span data-ttu-id="0aa31-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aa31-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="0aa31-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa31-133">Response</span></span>
<span data-ttu-id="0aa31-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0aa31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





