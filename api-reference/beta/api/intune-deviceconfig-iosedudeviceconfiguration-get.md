---
title: Obter iosEduDeviceConfiguration
description: Leia as propriedades e os relacionamentos do objeto iosEduDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93061a1321cc3c547d1b5f023f762c01d296ea56
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403949"
---
# <a name="get-iosedudeviceconfiguration"></a><span data-ttu-id="af05c-103">Obter iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="af05c-103">Get iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="af05c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="af05c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af05c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af05c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af05c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="af05c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af05c-107">Leia as propriedades e os relacionamentos do objeto [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="af05c-107">Read properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af05c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af05c-108">Prerequisites</span></span>
<span data-ttu-id="af05c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="af05c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="af05c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af05c-111">Permission type</span></span>|<span data-ttu-id="af05c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af05c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af05c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af05c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af05c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af05c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af05c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af05c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af05c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af05c-116">Not supported.</span></span>|
|<span data-ttu-id="af05c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af05c-117">Application</span></span>|<span data-ttu-id="af05c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af05c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af05c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af05c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af05c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af05c-120">Optional query parameters</span></span>
<span data-ttu-id="af05c-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af05c-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af05c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af05c-122">Request headers</span></span>
|<span data-ttu-id="af05c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af05c-123">Header</span></span>|<span data-ttu-id="af05c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="af05c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af05c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="af05c-125">Authorization</span></span>|<span data-ttu-id="af05c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af05c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af05c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af05c-127">Accept</span></span>|<span data-ttu-id="af05c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="af05c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af05c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af05c-129">Request body</span></span>
<span data-ttu-id="af05c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af05c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af05c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="af05c-131">Response</span></span>
<span data-ttu-id="af05c-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af05c-132">If successful, this method returns a `200 OK` response code and [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af05c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af05c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="af05c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af05c-134">Request</span></span>
<span data-ttu-id="af05c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af05c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="af05c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="af05c-136">Response</span></span>
<span data-ttu-id="af05c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af05c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2189

{
  "value": {
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
}
```




