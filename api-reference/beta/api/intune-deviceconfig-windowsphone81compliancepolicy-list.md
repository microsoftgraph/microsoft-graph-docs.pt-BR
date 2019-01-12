---
title: Listar windowsPhone81CompliancePolicies
description: Listar propriedades e relações dos objetos windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dcb72e1da83abe568d46b7a3d6578434a1b31876
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969153"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="53558-103">Listar windowsPhone81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="53558-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="53558-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53558-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53558-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53558-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53558-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53558-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53558-107">Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="53558-107">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53558-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53558-108">Prerequisites</span></span>
<span data-ttu-id="53558-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53558-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53558-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53558-111">Permission type</span></span>|<span data-ttu-id="53558-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53558-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53558-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53558-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53558-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="53558-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="53558-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53558-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53558-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53558-116">Not supported.</span></span>|
|<span data-ttu-id="53558-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53558-117">Application</span></span>|<span data-ttu-id="53558-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53558-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53558-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53558-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="53558-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53558-120">Request headers</span></span>
|<span data-ttu-id="53558-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53558-121">Header</span></span>|<span data-ttu-id="53558-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53558-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53558-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53558-123">Authorization</span></span>|<span data-ttu-id="53558-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53558-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53558-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53558-125">Accept</span></span>|<span data-ttu-id="53558-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53558-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53558-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53558-127">Request body</span></span>
<span data-ttu-id="53558-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53558-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53558-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="53558-129">Response</span></span>
<span data-ttu-id="53558-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53558-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53558-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53558-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="53558-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53558-132">Request</span></span>
<span data-ttu-id="53558-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53558-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="53558-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="53558-134">Response</span></span>
<span data-ttu-id="53558-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53558-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





