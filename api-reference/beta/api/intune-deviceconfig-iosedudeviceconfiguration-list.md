---
title: Lista iosEduDeviceConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosEduDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5d74a6a88e804156b47b005330119b5e12da033f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935014"
---
# <a name="list-iosedudeviceconfigurations"></a><span data-ttu-id="b9a56-103">Lista iosEduDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="b9a56-103">List iosEduDeviceConfigurations</span></span>

> <span data-ttu-id="b9a56-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9a56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9a56-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9a56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9a56-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9a56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9a56-107">Lista as propriedades e os relacionamentos dos objetos [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b9a56-107">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9a56-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9a56-108">Prerequisites</span></span>
<span data-ttu-id="b9a56-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a56-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a56-111">Permission type</span></span>|<span data-ttu-id="b9a56-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9a56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9a56-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9a56-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9a56-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9a56-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9a56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a56-116">Not supported.</span></span>|
|<span data-ttu-id="b9a56-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a56-117">Application</span></span>|<span data-ttu-id="b9a56-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9a56-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b9a56-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a56-120">Request headers</span></span>
|<span data-ttu-id="b9a56-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9a56-121">Header</span></span>|<span data-ttu-id="b9a56-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b9a56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9a56-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a56-123">Authorization</span></span>|<span data-ttu-id="b9a56-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9a56-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9a56-125">Accept</span></span>|<span data-ttu-id="b9a56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9a56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a56-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a56-127">Request body</span></span>
<span data-ttu-id="b9a56-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9a56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a56-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a56-129">Response</span></span>
<span data-ttu-id="b9a56-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a56-130">If successful, this method returns a `200 OK` response code and a collection of [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a56-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a56-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9a56-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a56-132">Request</span></span>
<span data-ttu-id="b9a56-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a56-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b9a56-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a56-134">Response</span></span>
<span data-ttu-id="b9a56-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9a56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





