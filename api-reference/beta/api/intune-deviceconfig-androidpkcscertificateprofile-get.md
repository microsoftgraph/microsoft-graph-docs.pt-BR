---
title: Obter androidPkcsCertificateProfile
description: Leia as propriedades e os relacionamentos do objeto androidPkcsCertificateProfile.
ms.openlocfilehash: 3f910c8d90e866e2646df2509b226b1d6bfd510b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036871"
---
# <a name="get-androidpkcscertificateprofile"></a><span data-ttu-id="5309d-103">Obter androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5309d-103">Get androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="5309d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5309d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5309d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5309d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5309d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5309d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5309d-107">Leia as propriedades e os relacionamentos do objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5309d-107">Read properties and relationships of the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5309d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5309d-108">Prerequisites</span></span>
<span data-ttu-id="5309d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5309d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5309d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5309d-111">Permission type</span></span>|<span data-ttu-id="5309d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5309d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5309d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5309d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5309d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5309d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5309d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5309d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5309d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5309d-116">Not supported.</span></span>|
|<span data-ttu-id="5309d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5309d-117">Application</span></span>|<span data-ttu-id="5309d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5309d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5309d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5309d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5309d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5309d-120">Optional query parameters</span></span>
<span data-ttu-id="5309d-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5309d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5309d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5309d-122">Request headers</span></span>
|<span data-ttu-id="5309d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5309d-123">Header</span></span>|<span data-ttu-id="5309d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5309d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5309d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5309d-125">Authorization</span></span>|<span data-ttu-id="5309d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5309d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5309d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5309d-127">Accept</span></span>|<span data-ttu-id="5309d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5309d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5309d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5309d-129">Request body</span></span>
<span data-ttu-id="5309d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5309d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5309d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5309d-131">Response</span></span>
<span data-ttu-id="5309d-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5309d-132">If successful, this method returns a `200 OK` response code and [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5309d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5309d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5309d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5309d-134">Request</span></span>
<span data-ttu-id="5309d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5309d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5309d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5309d-136">Response</span></span>
<span data-ttu-id="5309d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5309d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1203

{
  "value": {
    "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
    "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
    "subjectAlternativeNameType": "emailAddress",
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
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```





