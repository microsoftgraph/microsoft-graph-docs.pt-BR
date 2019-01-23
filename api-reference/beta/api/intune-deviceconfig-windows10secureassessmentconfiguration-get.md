---
title: Acessar windows10SecureAssessmentConfiguration
description: Leia as propriedades e relações de objetos de windows10SecureAssessmentConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a97729bcc841365dfacb3af3037c87b43e435ddf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393820"
---
# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="b9f81-103">Acessar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9f81-103">Get windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="b9f81-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9f81-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b9f81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9f81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9f81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b9f81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f81-107">Leia as propriedades e relações de objetos de [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9f81-107">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9f81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9f81-108">Prerequisites</span></span>
<span data-ttu-id="b9f81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9f81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9f81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9f81-111">Permission type</span></span>|<span data-ttu-id="b9f81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9f81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9f81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f81-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f81-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9f81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9f81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f81-116">Not supported.</span></span>|
|<span data-ttu-id="b9f81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9f81-117">Application</span></span>|<span data-ttu-id="b9f81-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9f81-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9f81-120">Optional query parameters</span></span>
<span data-ttu-id="b9f81-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f81-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9f81-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f81-122">Request headers</span></span>
|<span data-ttu-id="b9f81-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9f81-123">Header</span></span>|<span data-ttu-id="b9f81-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9f81-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f81-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9f81-125">Authorization</span></span>|<span data-ttu-id="b9f81-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9f81-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f81-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9f81-127">Accept</span></span>|<span data-ttu-id="b9f81-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f81-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f81-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f81-129">Request body</span></span>
<span data-ttu-id="b9f81-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9f81-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f81-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f81-131">Response</span></span>
<span data-ttu-id="b9f81-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f81-132">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f81-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9f81-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9f81-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f81-134">Request</span></span>
<span data-ttu-id="b9f81-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9f81-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b9f81-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f81-136">Response</span></span>
<span data-ttu-id="b9f81-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9f81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 724

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
    "id": "f60d71be-71be-f60d-be71-0df6be710df6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "launchUri": "Launch Uri value",
    "configurationAccount": "Configuration Account value",
    "configurationAccountType": "domainAccount",
    "allowPrinting": true,
    "allowScreenCapture": true,
    "allowTextSuggestion": true
  }
}
```




