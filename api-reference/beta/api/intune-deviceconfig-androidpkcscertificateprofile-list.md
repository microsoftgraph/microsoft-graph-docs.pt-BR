---
title: Listar androidPkcsCertificateProfiles
description: Listar Propriedades e relações dos objetos androidPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04c8473e6445c801535b815c5333f80503f1adb3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155122"
---
# <a name="list-androidpkcscertificateprofiles"></a><span data-ttu-id="71c64-103">Listar androidPkcsCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="71c64-103">List androidPkcsCertificateProfiles</span></span>

> <span data-ttu-id="71c64-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71c64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71c64-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71c64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c64-106">Listar Propriedades e relações dos objetos [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="71c64-106">List properties and relationships of the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71c64-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71c64-107">Prerequisites</span></span>
<span data-ttu-id="71c64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71c64-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71c64-110">Permission type</span></span>|<span data-ttu-id="71c64-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71c64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c64-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71c64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71c64-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71c64-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71c64-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71c64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c64-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71c64-115">Not supported.</span></span>|
|<span data-ttu-id="71c64-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71c64-116">Application</span></span>|<span data-ttu-id="71c64-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71c64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c64-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71c64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71c64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71c64-119">Request headers</span></span>
|<span data-ttu-id="71c64-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71c64-120">Header</span></span>|<span data-ttu-id="71c64-121">Valor</span><span class="sxs-lookup"><span data-stu-id="71c64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c64-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71c64-122">Authorization</span></span>|<span data-ttu-id="71c64-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71c64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c64-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71c64-124">Accept</span></span>|<span data-ttu-id="71c64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71c64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c64-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71c64-126">Request body</span></span>
<span data-ttu-id="71c64-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71c64-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71c64-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="71c64-128">Response</span></span>
<span data-ttu-id="71c64-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71c64-129">If successful, this method returns a `200 OK` response code and a collection of [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c64-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71c64-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="71c64-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71c64-131">Request</span></span>
<span data-ttu-id="71c64-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71c64-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="71c64-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="71c64-133">Response</span></span>
<span data-ttu-id="71c64-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71c64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1271

{
  "value": [
    {
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
  ]
}
```




