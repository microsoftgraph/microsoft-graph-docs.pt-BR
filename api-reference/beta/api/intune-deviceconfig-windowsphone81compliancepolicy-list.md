---
title: Listar windowsPhone81CompliancePolicies
description: Listar propriedades e relações dos objetos windowsPhone81CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: c7ce1588e9be2258f81b89c961b5eb67cb499ee6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361548"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="d1932-103">Listar windowsPhone81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="d1932-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="d1932-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1932-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1932-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1932-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1932-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d1932-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1932-107">Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d1932-107">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1932-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1932-108">Prerequisites</span></span>
<span data-ttu-id="d1932-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1932-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1932-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1932-111">Permission type</span></span>|<span data-ttu-id="d1932-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1932-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1932-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1932-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1932-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1932-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d1932-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1932-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1932-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1932-116">Not supported.</span></span>|
|<span data-ttu-id="d1932-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1932-117">Application</span></span>|<span data-ttu-id="d1932-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1932-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1932-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1932-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d1932-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1932-120">Request headers</span></span>
|<span data-ttu-id="d1932-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1932-121">Header</span></span>|<span data-ttu-id="d1932-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1932-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1932-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1932-123">Authorization</span></span>|<span data-ttu-id="d1932-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1932-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1932-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1932-125">Accept</span></span>|<span data-ttu-id="d1932-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1932-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1932-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1932-127">Request body</span></span>
<span data-ttu-id="d1932-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1932-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1932-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1932-129">Response</span></span>
<span data-ttu-id="d1932-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1932-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1932-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1932-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1932-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1932-132">Request</span></span>
<span data-ttu-id="d1932-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1932-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d1932-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1932-134">Response</span></span>
<span data-ttu-id="d1932-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1932-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
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
  ]
}
```





