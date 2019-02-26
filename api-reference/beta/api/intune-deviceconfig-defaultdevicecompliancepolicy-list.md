---
title: Listar defaultDeviceCompliancePolicies
description: Listar Propriedades e relações dos objetos defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c76fcb88f39bd965d36f24cb44ba429bab23f0c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166273"
---
# <a name="list-defaultdevicecompliancepolicies"></a><span data-ttu-id="bc725-103">Listar defaultDeviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="bc725-103">List defaultDeviceCompliancePolicies</span></span>

> <span data-ttu-id="bc725-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc725-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc725-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc725-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc725-106">Listar Propriedades e relações dos objetos [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bc725-106">List properties and relationships of the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc725-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc725-107">Prerequisites</span></span>
<span data-ttu-id="bc725-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc725-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc725-110">Permission type</span></span>|<span data-ttu-id="bc725-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc725-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc725-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc725-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc725-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc725-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bc725-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc725-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc725-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc725-115">Not supported.</span></span>|
|<span data-ttu-id="bc725-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc725-116">Application</span></span>|<span data-ttu-id="bc725-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc725-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc725-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc725-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bc725-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc725-119">Request headers</span></span>
|<span data-ttu-id="bc725-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc725-120">Header</span></span>|<span data-ttu-id="bc725-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bc725-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc725-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc725-122">Authorization</span></span>|<span data-ttu-id="bc725-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc725-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc725-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc725-124">Accept</span></span>|<span data-ttu-id="bc725-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc725-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc725-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc725-126">Request body</span></span>
<span data-ttu-id="bc725-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc725-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc725-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc725-128">Response</span></span>
<span data-ttu-id="bc725-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc725-129">If successful, this method returns a `200 OK` response code and a collection of [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc725-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc725-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc725-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc725-131">Request</span></span>
<span data-ttu-id="bc725-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc725-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="bc725-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc725-133">Response</span></span>
<span data-ttu-id="bc725-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc725-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




