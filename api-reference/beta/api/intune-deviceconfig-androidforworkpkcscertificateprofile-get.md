---
title: Obter androidForWorkPkcsCertificateProfile
description: Leia as propriedades e os relacionamentos do objeto androidForWorkPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dff72d78a51b4c74071c51fdb81bc7a68c6ca407
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990144"
---
# <a name="get-androidforworkpkcscertificateprofile"></a><span data-ttu-id="2df25-103">Obter androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2df25-103">Get androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="2df25-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2df25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2df25-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2df25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2df25-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2df25-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df25-107">Leia as propriedades e os relacionamentos do objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2df25-107">Read properties and relationships of the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df25-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2df25-108">Prerequisites</span></span>
<span data-ttu-id="2df25-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df25-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df25-111">Permission type</span></span>|<span data-ttu-id="2df25-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2df25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df25-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2df25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2df25-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df25-116">Not supported.</span></span>|
|<span data-ttu-id="2df25-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df25-117">Application</span></span>|<span data-ttu-id="2df25-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df25-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df25-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2df25-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2df25-120">Optional query parameters</span></span>
<span data-ttu-id="2df25-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2df25-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2df25-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df25-122">Request headers</span></span>
|<span data-ttu-id="2df25-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2df25-123">Header</span></span>|<span data-ttu-id="2df25-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2df25-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df25-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df25-125">Authorization</span></span>|<span data-ttu-id="2df25-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df25-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df25-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2df25-127">Accept</span></span>|<span data-ttu-id="2df25-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2df25-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df25-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df25-129">Request body</span></span>
<span data-ttu-id="2df25-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2df25-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df25-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df25-131">Response</span></span>
<span data-ttu-id="2df25-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df25-132">If successful, this method returns a `200 OK` response code and [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df25-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df25-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df25-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df25-134">Request</span></span>
<span data-ttu-id="2df25-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df25-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2df25-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df25-136">Response</span></span>
<span data-ttu-id="2df25-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df25-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1210

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
    "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "renewalThresholdPercentage": 10,
    "subjectNameFormat": "commonNameIncludingEmail",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
    "subjectAlternativeNameType": "emailAddress"
  }
}
```





