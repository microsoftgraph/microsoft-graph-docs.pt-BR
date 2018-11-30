---
title: Get windowsPhone81CompliancePolicy
description: Ler propriedades e relações do objeto windowsPhone81CompliancePolicy.
ms.openlocfilehash: d68ac6dea545787dd3aa9fab7440e3febbf4a183
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035091"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="b9424-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b9424-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="b9424-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9424-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9424-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9424-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9424-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9424-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9424-107">Ler propriedades e relações do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b9424-107">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9424-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9424-108">Prerequisites</span></span>
<span data-ttu-id="b9424-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9424-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9424-111">Permission type</span></span>|<span data-ttu-id="b9424-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9424-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9424-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9424-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9424-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9424-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9424-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9424-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9424-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9424-116">Not supported.</span></span>|
|<span data-ttu-id="b9424-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9424-117">Application</span></span>|<span data-ttu-id="b9424-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9424-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9424-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9424-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9424-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9424-120">Optional query parameters</span></span>
<span data-ttu-id="b9424-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9424-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9424-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9424-122">Request headers</span></span>
|<span data-ttu-id="b9424-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9424-123">Header</span></span>|<span data-ttu-id="b9424-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9424-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9424-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9424-125">Authorization</span></span>|<span data-ttu-id="b9424-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9424-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9424-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b9424-127">Accept</span></span>|<span data-ttu-id="b9424-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9424-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9424-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9424-129">Request body</span></span>
<span data-ttu-id="b9424-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9424-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9424-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9424-131">Response</span></span>
<span data-ttu-id="b9424-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9424-132">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9424-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9424-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9424-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9424-134">Request</span></span>
<span data-ttu-id="b9424-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9424-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="b9424-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9424-136">Response</span></span>
<span data-ttu-id="b9424-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9424-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 902

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```





