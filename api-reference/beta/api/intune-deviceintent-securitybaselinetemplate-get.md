---
title: Obter securityBaselineTemplate
description: Leia propriedades e relações do objeto securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f3d8d44eb9aac33a1d4946146c4f641198b199d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154445"
---
# <a name="get-securitybaselinetemplate"></a><span data-ttu-id="8f111-103">Obter securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="8f111-103">Get securityBaselineTemplate</span></span>

<span data-ttu-id="8f111-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f111-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f111-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f111-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f111-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f111-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f111-107">Leia propriedades e relações do [objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8f111-107">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f111-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f111-108">Prerequisites</span></span>
<span data-ttu-id="8f111-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f111-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f111-111">Permission type</span></span>|<span data-ttu-id="8f111-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f111-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f111-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f111-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f111-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f111-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f111-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f111-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f111-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f111-116">Not supported.</span></span>|
|<span data-ttu-id="8f111-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f111-117">Application</span></span>|<span data-ttu-id="8f111-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f111-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f111-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f111-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f111-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f111-120">Optional query parameters</span></span>
<span data-ttu-id="8f111-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f111-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f111-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f111-122">Request headers</span></span>
|<span data-ttu-id="8f111-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f111-123">Header</span></span>|<span data-ttu-id="8f111-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8f111-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f111-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f111-125">Authorization</span></span>|<span data-ttu-id="8f111-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f111-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f111-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f111-127">Accept</span></span>|<span data-ttu-id="8f111-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8f111-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f111-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f111-129">Request body</span></span>
<span data-ttu-id="8f111-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f111-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f111-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f111-131">Response</span></span>
<span data-ttu-id="8f111-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um objeto securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f111-132">If successful, this method returns a `200 OK` response code and [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f111-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f111-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f111-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f111-134">Request</span></span>
<span data-ttu-id="8f111-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f111-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="8f111-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f111-136">Response</span></span>
<span data-ttu-id="8f111-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f111-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineTemplate",
    "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
    "displayName": "Display Name value",
    "description": "Description value",
    "versionInfo": "Version Info value",
    "isDeprecated": true,
    "intentCount": 11,
    "templateType": "specializedDevices",
    "platformType": "androidForWork",
    "templateSubtype": "firewall",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
  }
}
```




