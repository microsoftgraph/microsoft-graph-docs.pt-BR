---
title: Listar windows81CompliancePolicies
description: Listar propriedades e relações dos objetos windows81CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 217ec11f7c2283d8eae90129896b00823211da81
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333072"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="d3d0e-103">Listar windows81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="d3d0e-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="d3d0e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3d0e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3d0e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3d0e-107">Listar propriedades e relações dos objetos [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d3d0e-107">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3d0e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3d0e-108">Prerequisites</span></span>
<span data-ttu-id="d3d0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3d0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3d0e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3d0e-111">Permission type</span></span>|<span data-ttu-id="d3d0e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3d0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3d0e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3d0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3d0e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3d0e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d3d0e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3d0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3d0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-116">Not supported.</span></span>|
|<span data-ttu-id="d3d0e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3d0e-117">Application</span></span>|<span data-ttu-id="d3d0e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3d0e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3d0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d3d0e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d0e-120">Request headers</span></span>
|<span data-ttu-id="d3d0e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3d0e-121">Header</span></span>|<span data-ttu-id="d3d0e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3d0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3d0e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3d0e-123">Authorization</span></span>|<span data-ttu-id="d3d0e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3d0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3d0e-125">Accept</span></span>|<span data-ttu-id="d3d0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3d0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3d0e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d0e-127">Request body</span></span>
<span data-ttu-id="d3d0e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3d0e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3d0e-129">Response</span></span>
<span data-ttu-id="d3d0e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-130">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3d0e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3d0e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3d0e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d0e-132">Request</span></span>
<span data-ttu-id="d3d0e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d3d0e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3d0e-134">Response</span></span>
<span data-ttu-id="d3d0e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3d0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 953

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```





