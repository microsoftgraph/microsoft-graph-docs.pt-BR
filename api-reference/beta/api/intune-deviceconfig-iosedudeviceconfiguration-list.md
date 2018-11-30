---
title: Lista iosEduDeviceConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosEduDeviceConfiguration.
ms.openlocfilehash: ed9d6aebcc0437d21bd64027dc41092f9e5fb471
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036764"
---
# <a name="list-iosedudeviceconfigurations"></a><span data-ttu-id="3e969-103">Lista iosEduDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="3e969-103">List iosEduDeviceConfigurations</span></span>

> <span data-ttu-id="3e969-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e969-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e969-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e969-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e969-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e969-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e969-107">Lista as propriedades e os relacionamentos dos objetos [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3e969-107">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e969-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e969-108">Prerequisites</span></span>
<span data-ttu-id="3e969-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e969-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e969-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e969-111">Permission type</span></span>|<span data-ttu-id="3e969-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e969-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e969-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e969-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e969-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e969-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3e969-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e969-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e969-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e969-116">Not supported.</span></span>|
|<span data-ttu-id="3e969-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e969-117">Application</span></span>|<span data-ttu-id="3e969-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e969-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e969-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e969-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e969-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e969-120">Request headers</span></span>
|<span data-ttu-id="3e969-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e969-121">Header</span></span>|<span data-ttu-id="3e969-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3e969-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e969-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e969-123">Authorization</span></span>|<span data-ttu-id="3e969-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e969-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e969-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e969-125">Accept</span></span>|<span data-ttu-id="3e969-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e969-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e969-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e969-127">Request body</span></span>
<span data-ttu-id="3e969-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e969-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e969-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e969-129">Response</span></span>
<span data-ttu-id="3e969-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e969-130">If successful, this method returns a `200 OK` response code and a collection of [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e969-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e969-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e969-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e969-132">Request</span></span>
<span data-ttu-id="3e969-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e969-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3e969-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e969-134">Response</span></span>
<span data-ttu-id="3e969-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e969-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2291

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
      "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "teacherCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      },
      "studentCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      },
      "deviceCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      }
    }
  ]
}
```





