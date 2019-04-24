---
title: Obter androidForWorkCertificateProfileBase
description: Leia as propriedades e as relações do objeto androidForWorkCertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6401768042a8682a3a56548ed3ab64097b3dee3d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479341"
---
# <a name="get-androidforworkcertificateprofilebase"></a><span data-ttu-id="c44df-103">Obter androidForWorkCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="c44df-103">Get androidForWorkCertificateProfileBase</span></span>

> <span data-ttu-id="c44df-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c44df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c44df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c44df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c44df-106">Leia as propriedades e as relações do objeto [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="c44df-106">Read properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c44df-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c44df-107">Prerequisites</span></span>
<span data-ttu-id="c44df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c44df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c44df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c44df-110">Permission type</span></span>|<span data-ttu-id="c44df-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c44df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c44df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c44df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c44df-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c44df-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c44df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c44df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c44df-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c44df-115">Not supported.</span></span>|
|<span data-ttu-id="c44df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c44df-116">Application</span></span>|<span data-ttu-id="c44df-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c44df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c44df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c44df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEasEmailProfileBase/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c44df-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c44df-119">Optional query parameters</span></span>
<span data-ttu-id="c44df-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c44df-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c44df-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c44df-121">Request headers</span></span>
|<span data-ttu-id="c44df-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c44df-122">Header</span></span>|<span data-ttu-id="c44df-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c44df-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c44df-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c44df-124">Authorization</span></span>|<span data-ttu-id="c44df-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c44df-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c44df-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c44df-126">Accept</span></span>|<span data-ttu-id="c44df-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c44df-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c44df-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c44df-128">Request body</span></span>
<span data-ttu-id="c44df-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c44df-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c44df-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c44df-130">Response</span></span>
<span data-ttu-id="c44df-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c44df-131">If successful, this method returns a `200 OK` response code and [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c44df-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c44df-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c44df-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c44df-133">Request</span></span>
<span data-ttu-id="c44df-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c44df-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
```

### <a name="response"></a><span data-ttu-id="c44df-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c44df-135">Response</span></span>
<span data-ttu-id="c44df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c44df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 915

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkCertificateProfileBase",
    "id": "87f1d53b-d53b-87f1-3bd5-f1873bd5f187",
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
    "subjectAlternativeNameType": "emailAddress"
  }
}
```





