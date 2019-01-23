---
title: Obter windows81CertificateProfileBase
description: Leia as propriedades e os relacionamentos do objeto windows81CertificateProfileBase.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8f232f5dd0e6fff7b9a993995315f44dfdb4e2a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410529"
---
# <a name="get-windows81certificateprofilebase"></a><span data-ttu-id="e1776-103">Obter windows81CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="e1776-103">Get windows81CertificateProfileBase</span></span>

> <span data-ttu-id="e1776-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1776-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1776-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1776-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1776-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e1776-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1776-107">Leia as propriedades e os relacionamentos do objeto [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="e1776-107">Read properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1776-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1776-108">Prerequisites</span></span>
<span data-ttu-id="e1776-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1776-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1776-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1776-111">Permission type</span></span>|<span data-ttu-id="e1776-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1776-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1776-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1776-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1776-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1776-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1776-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1776-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1776-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1776-116">Not supported.</span></span>|
|<span data-ttu-id="e1776-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1776-117">Application</span></span>|<span data-ttu-id="e1776-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1776-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1776-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1776-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1776-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1776-120">Optional query parameters</span></span>
<span data-ttu-id="e1776-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1776-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1776-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1776-122">Request headers</span></span>
|<span data-ttu-id="e1776-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1776-123">Header</span></span>|<span data-ttu-id="e1776-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e1776-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1776-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1776-125">Authorization</span></span>|<span data-ttu-id="e1776-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1776-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1776-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1776-127">Accept</span></span>|<span data-ttu-id="e1776-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e1776-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1776-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1776-129">Request body</span></span>
<span data-ttu-id="e1776-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1776-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1776-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1776-131">Response</span></span>
<span data-ttu-id="e1776-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1776-132">If successful, this method returns a `200 OK` response code and [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1776-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1776-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1776-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1776-134">Request</span></span>
<span data-ttu-id="e1776-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1776-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1776-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1776-136">Response</span></span>
<span data-ttu-id="e1776-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1776-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1167

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
    "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
    "keyStorageProvider": "useTpmKspOtherwiseFail",
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
    "customSubjectAlternativeNames": [
      {
        "@odata.type": "microsoft.graph.customSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ]
  }
}
```




